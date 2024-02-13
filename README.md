# expo-workflows
A collection of workflows that use Expo and EAS to build React Native apps.

# contributing
Please feel free to provide your own workflows that may be useful to other people, or any improvements you have to existing ones. For more information, please see the [contributing file](./CONTRIBUTING.md).

# usage
> **WARNING"" - these builds take around 10-20 minutes to run. Please be wary of your GitHub actions allowance to avoid incurring any unintentional costs.

Add the workflow you want to use to the `.github/workflows` directory in your own repo. Specify in the file what you want to trigger the build, further information can be found [here](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows). Add your Expo token to the `EXPO_TOKEN` repository secret in the repository settings, more information on this can be found [here](https://github.com/expo/expo-github-action?tab=readme-ov-file).

> **NOTE** - you will need to have build credentials uploaded to EAS in order for these builds to work

# android
`android-production-build.yml` - builds an AAB using your signing credentials that are stored in EAS. Once workflow has completed, the artifact is accessible under the workflow run.
<br/>
<br/>
`android-apk-build.yml` - builds a preview APK. Once workflow has completed, the artifact is accessible under the workflow run.

![alt text](image.png)

# ios
`ios-production-build.yml` - builds an IPA using your signing credentials and provisioning profile that are stored in EAS. Once workflow has completed, the artifact is accessible under the workflow run. You can submit this file to the app store by using EAS submit.
