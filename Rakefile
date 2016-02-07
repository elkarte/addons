require 'html/proofer'

task :test do
  HTML::Proofer.new("./_site", check_html: false, validation: { ignore_script_embeds: true }, checks_to_ignore: ['LinkCheck'], only_4xx: true, href_ignore: ['#'], disable_external: true, empty_alt_ignore: true, ssl_verifypeer: false).run
end