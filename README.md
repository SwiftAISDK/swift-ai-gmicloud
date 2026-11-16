<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-gmicloud 1.2.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-gmicloud.git", from: "1.2.0")
```

Products: `SwiftAIGMICloud`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# GMI Cloud for Swift

`SwiftAIGMICloud` adds GMI Cloud to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/gmicloud` and supports text generation.

Provider guide with models, options, streaming and errors:

- [GMI Cloud](https://swiftaisdk.github.io/SwiftAISDK/providers/gmicloud/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIGMICloud` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIGMICloud

let provider = try AIProviders.gmiCloud(configuration: GMICloudProviderSettings())
```

By default the provider reads `GMI_CLOUD_APIKEY` from the environment; values set in `GMICloudProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-gmicloud` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
