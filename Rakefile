SSH = 'ssh -A -i ~/git/bitfield/bitfield.pem -l ubuntu1'

desc "Run Puppet on ENV['CLIENT']"
task :apply do
	client = ENV['CLIENT']
	sh "git push"
	sh "#{SSH} #{client} pull-updates"
end
