source 'https://cdn.cocoapods.org/'
install! 'cocoapods', :warn_for_unused_master_specs_repo => false

$minimum_deployment_version = '15.0'

platform :ios, $minimum_deployment_version

target 'Flash Chat iOS15' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Flash Chat iOS15
  pod 'CLTypingLabel',' ~> 0.4.0'
  pod 'FirebaseAuth'
  pod 'FirebaseFirestore'

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = $minimum_deployment_version
    end
  end
end
