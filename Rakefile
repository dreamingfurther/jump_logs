# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require_relative 'config/application'

Rails.application.load_tasks
Rake.application['default'].prerequisites.delete('spec') if Rake.application['default']

task default: ['spec:frontend', 'spec:units', 'spec:features']
