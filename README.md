# OneUI Icons

Currently, `957` icons are available (13.07.2022). Special thanks to [Maulana990](https://github.com/Maulana990).

You can get all the icons either as a [library](#library), include them [directly in Android Studio](#android-studios-asset-studio) or as [single files](#alternative). 

## Library

<a href="https://mvnrepository.com/artifact/io.github.oneuiproject/icons"><img src="https://img.shields.io/maven-central/v/io.github.oneuiproject/icons?color=%23C71A36&label=Maven&logo=Apache%20Maven&logoColor=%23C11920&style=for-the-badge"/></a>

Add the library in your dependencies and all the OneUI icon names start with `ic_oui`.
```groovy
dependencies {
    // ...
    implementation 'io.github.oneuiproject:icons:<version>'
}
```

## Android Studio's Asset Studio

<p align="center">
  <img src="readme-res/asset_studio.png" width="80%"/>
</p>

Pick oneui icons directly from Android Studio's Asset Studio by going to `File > New > Vector Asset > Clip Art` and searching for `oui`.

For this to work, you need to download [material.zip](https://github.com/OneUIProject/oneui-icons/raw/main/material.zip) and extract it to `<android_sdk_dir>/icons/material/`. Replace `icons_metadata.txt` and merge the contents of `materialicons`.

Default SDK location:
- Windows: `C:/Users/<username>/AppData/Local/Android/Sdk/`
- MacOS: `/Users/<username>/Library/Android/sdk/`
- Linux: `/home/<username>/Android/Sdk/`

After you've extracted the zip you can open the Asset Studio and find all the oneui icons by searching for `oui`.

**Notes:**
- The Asset Studio will add a tint to the drawable. Simply remove it if you need the colors.
- Some icons might not work, in this case you can also get them from [below](#alternative). (I'm working on a fix)

## Alternative
If you're not using Android Studio or need them as a file you can get them all [here](lib\src\main\res\drawable).