require 'html/proofer'

task :test do
  HTML::Proofer.new("./_site", only_4xx: true, check_html: true, href_ignore: ['#'], ssl_verifypeer: false).run
end