desc "Run the test suite"

task :test do
  build = "xcodebuild \
    -workspace Tests/Tests.xcworkspace \
    -scheme Tests \
    -sdk iphonesimulator -destination 'platform=iOS Simulator,name=iPhone 6,OS=8.1'"
  system "#{build} test | xcpretty --test --color"  
end

task :default => :test

