# Uncomment the next line to define a global platform for your project
platform :ios, '9.0'

target 'XML文件解析' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  
   pod 'KissXML'

   # 更改所有第三方框架 Target 版本
   post_install do |installer|
     installer.pods_project.targets.each do |target|
       target.build_configurations.each do |config|
         config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
         config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
         config.build_settings['CODE_SIGN_IDENTITY'] = ''
       end
     end
   end

  # Pods for XML文件解析

  target 'XML文件解析Tests' do
    # Pods for testing
  end

  target 'XML文件解析UITests' do
    # Pods for testing
  end

end
