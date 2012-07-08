$:.unshift("/Library/RubyMotion/lib")
require 'motion/project'
require 'bundler'
Bundler.setup
Bundler.require

Motion::Project::App.setup do |app|
  app.name = 'iPOuL'
  app.identifier = 'com.thmdev.ipoul'
  app.version = '3.1'
  app.short_version = '3.1'
  app.device_family = [:iphone, :ipad]
  app.frameworks += ['MapKit']
  app.pods do
    dependency 'SVPullToRefresh'
  end
  app.icons = %w{Icon Icon@2x Icon-72 Icon-Small Icon-Small@2x }
  app.codesign_certificate = "iPhone Distribution: Maxim S.N.C. Di D'Amico Giuseppe & C."
  app.provisioning_profile = "/Users/Simone/Library/MobileDevice/Provisioning Profiles/72F8E8EB-EC61-4762-AB21-9AA31CBE4799.mobileprovision"
end
