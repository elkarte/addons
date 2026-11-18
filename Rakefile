require "html-proofer"

task :test do
  options = {
    disable_external: true,
    ignore_empty_alt: true,
    ignore_urls: ["#"],
    # The site's baseurl is an absolute URL, so strip it to resolve links
    # against the locally generated _site directory.
    swap_urls: { %r{^https://addons\.elkarte\.net} => "" }
  }

  HTMLProofer.check_directory("./_site", options).run
end
