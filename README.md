# expo-workflows
A collection of workflows that use Expo and EAS to build React Native apps.

# usage
Add the workflow you want to use to the `.github/workflows` directory in your own repo. Specify in the file what you want to trigger the build, further information can be found [here](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows). Add your Expo token to the `EXPO_TOKEN` repository secret in the repository settings, more information on this can be found [here](https://github.com/expo/expo-github-action?tab=readme-ov-file).

# android
`android-production-build.yml` - builds an AAB using your siging credentials that are stored in EAS. Once workflow has completed, the artifact is accessible under the workflow run.

![alt text](image.png)