require 'puppetlabs_spec_helper/rake_tasks'
require 'puppet-syntax/tasks/puppet-syntax'
require 'puppet-lint/tasks/puppet-lint'

PuppetSyntax.exclude_paths = ["spec/fixtures/**/*"]
PuppetLint.configuration.send("disable_class_inherits_from_params_class")
PuppetLint.configuration.ignore_paths = ["spec/**/*.pp", 'tests/**/*.pp']

task :default => [
  :syntax,
  :lint,
  :spec,
]
