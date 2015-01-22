# Guardfile

require 'asciidoctor'
require 'erb'

guard 'shell' do
watch(/^*\.adoc$/) {|m|
  Asciidoctor.render_file('idris-tutorial.adoc', :safe => :unsafe, :in_place => true)
}
end

guard 'livereload' do
  watch(%r{^.+\.(css|js|html)$})
end
