# kottie
A cli tool based on Koltin/Native to convert your Lottie JSON to dotLottie format.

```shell
./kottie -h
Usage: kottie [<options>] [<files>]...

  Convert Lottie JSON to dotLottie format

Options:
  -r, --recursive  convert directories recursively
  -h, --help       Show this message and exit
```

## Config cookie
LottieFiles modified the API for converting and requires authorization. So you need to config your LottieFiles cookie manually: 
1. Open [Convert Lottie JSON](https://lottiefiles.com/tools/lottie-to-dotlottie) and login with your account
2. Open the developer console and go to the application tab
3. Get the value for name `ory_kratos_session` under site https://lottiefiles.com/
4. Save your cookie to the file `~/.kottie/cookie` with format `ory_kratos_session={your_session_value}`
5. Enjoy

## Release
1. Setup your build environment [Get started with Kotlin/Native in IntelliJ IDEA](https://kotlinlang.org/docs/native-get-started.html)
2. `./gradlew clean assembleReleaseExecutableMacos`

### Thanks to
- [Koltin/Native](https://kotlinlang.org/docs/native-overview.html)
- [kotlinx.coroutines](https://github.com/Kotlin/kotlinx.coroutines)
- [kotlinx.serialization](https://github.com/Kotlin/kotlinx.serialization)
- [Clikt](https://github.com/ajalt/clikt)
- [Okio](https://github.com/square/okio)
- [Ktor](https://ktor.io/)
- [to-dot-lottie](https://github.com/theapache64/to-dot-lottie)
- [.Lottie](https://dotlottie.io/)
