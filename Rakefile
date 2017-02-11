require 'fileutils'

@output = '/var/www/joda-project/'
@cdn = '/var/www/cdn/'
@cdn_name = 'joda-project'

task default: %w(serve)

task :serve do
  puts `bundle exec jekyll serve --watch`
end

task :deploy do
  puts 'Building web page using Jekyll'

  puts `JEKYLL_ENV=production bundle exec jekyll build --config _config.yml,_production.yml --destination #{@output}`

  puts ''
  puts 'Copying assets and other resources to CDN'

  FileUtils.rm_rf("#{@cdn}#{@cdn_name}/")

  FileUtils.mkdir("#{@cdn}#{@cdn_name}")
  FileUtils.cp_r "#{@output}assets/", "#{@cdn}#{@cdn_name}/assets", verbose: true
end
