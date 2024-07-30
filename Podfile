source 'https://mirrors.tuna.tsinghua.edu.cn/git/CocoaPods/Specs.git'
# source "https://github.com/CocoaPods/Specs.git"
platform :ios, "12.0"
use_frameworks!

target "DanTang" do
pod 'SVProgressHUD'
pod 'FDFullscreenPopGesture', '~> 1.1'
pod 'SnapKit', '~> 4.2.0'
pod 'Kingfisher', '~> 7.0'
pod 'Alamofire', '~> 4.3.0'
pod 'SwiftyJSON', '~> 4.0'

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings["IPHONEOS_DEPLOYMENT_TARGET"] = "12.0"
    end
  end
end
