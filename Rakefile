# frozen_string_literal: true

require "bundler/gem_tasks"
require "rspec/core/rake_task"
require "github_changelog_generator/task"
require "ams_lazy_relationships/version"

RSpec::Core::RakeTask.new(:spec)

task default: :spec

GitHubChangelogGenerator::RakeTask.new :changelog do |config|
  config.user = "Bajena"
  config.project = "ams_lazy_relationships"
  config.future_release = "v#{AmsLazyRelationships::VERSION}"
end
