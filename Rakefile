require 'html/proofer'

task :test do
  HTML::Proofer.new("./_site", href_ignore: ['#'], ssl_verifypeer: false, validate_html: true).run
end