# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

use_frameworks!

# ignore all warnings from all pods
inhibit_all_warnings!

workspace 'Tinodios'

project 'Tinodios'
project 'TinodeSDK'

def sdk_pods
    pod 'SwiftWebSocket', '~> 2.7.0'
end

def ui_pods
    pod 'SQLite.swift', '~> 0.11.5'
    pod 'MessageKit', '~> 2.0.0'
    pod 'MessageInputBar', '~> 0.4.1'
    pod 'SwiftKeychainWrapper', '~> 3.2'
end

target 'TinodeSDK' do
    project 'TinodeSDK'
    sdk_pods
end

target 'Tinodios' do
    project 'Tinodios'
    sdk_pods
    ui_pods
end
