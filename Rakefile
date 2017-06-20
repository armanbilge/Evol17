require 'rake/clean'

CLEAN.include '*.aux'
CLEAN.include '*.log'
CLEAN.include '*.out'

task :default => 'evol17.pdf'

file 'evol17.pdf' => ['evol17.tex']
CLOBBER.include 'evol17.pdf'

rule '.pdf' => '.tex' do |t|
  sh "pdflatex #{t.source}"
end
