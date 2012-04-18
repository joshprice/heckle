# -*- ruby -*-

require 'rubygems'
require 'hoe'

Hoe.add_include_dirs("../../ParseTree/dev/lib",
                     "../../ParseTree/dev/test",
                     "../../RubyInline/dev/lib",
                     "../../ruby2ruby/1.3.1/lib",
                     "../../ZenTest/dev/lib",
                     "../../sexp_processor/dev/lib",
                     "lib")

Hoe.plugin :seattlerb

Hoe.spec 'heckle' do
  developer 'Ryan Davis', 'ryand-ruby@zenspider.com'
  developer 'Eric Hodel', 'drbrain@segment7.net'
  developer 'Kevin Clark', 'kevin.clark@gmail.com'

  self.rubyforge_name = 'seattlerb'

  clean_globs << File.expand_path("~/.ruby_inline")

  dependency 'ParseTree', '~> 2.2.0'
  dependency 'ruby2ruby', '~> 1.3.0'
  dependency 'ZenTest',   '~> 4.7.0'

  multiruby_skip << "1.9" << "trunk"
end

# vim: syntax=ruby
