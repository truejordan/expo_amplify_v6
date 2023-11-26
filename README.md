### Amplify v6 compatibility issue

Error: The package '@aws-amplify/react-native' doesn't seem to be linked. Make sure:

- You have run 'pod install'
- You rebuilt the app after installing the package
- You are not using Expo Go
  , js engine: hermes

error is removed if we comment out lines use to congfigre amplify in root of app:
`
import { Amplify } from 'aws-amplify';
import amplifyconfig from '../src/amplifyconfiguration.json';
Amplify.configure(amplifyconfig);
`
