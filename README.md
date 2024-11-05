<h1 align="center">
  <br>
  <a href="https://ryUWUjinx.org/"><img src="https://media.discordapp.net/attachments/1263960833319239745/1292554586858459146/MpXwm0D.png?ex=672bb5c4&is=672a6444&hm=25b8ba06ec5eecb67b7ac7fb8540c1730dd198262366e1b45b3f1ada729b3c79&=&format=webp&quality=lossless" width="150"></a>
  <br>
  <b>RyUWUjinx</b>
  <br>
  <sub><sup><b>(REE-UWU-JINX)</b></sup></sub>
  <br>
</h1>

<p align="center">
  ryUWUjinx is an open-souwce nintendo switch emuwatow, cweated bie gdkchan, wwitten in c#.
   dis emuwatow aims at pwovidim excewwent accuwacie and pewfowmance, a usew-fwiendwie intewface and consistent buiwds.
   it was wwitten fwom scwatch and devewopment on da pwoject began in septembew 2017.
   ryUWUjinx is avaiwabwe on github undew da <a href="https://github.com/ryUWUjinx/ryUWUjinx/blob/master/LICENSE.txt" target="_blank">MIT license</a>.
<br />
</p>

<p align="center">
    <a href="https://github.com/ryUWUjinx/ryUWUjinx/actions/workflows/release.yml">
        <img src="https://github.com/ryUWUjinx/ryUWUjinx/actions/workflows/release.yml/badge.svg"
            alt="">
    </a>
    <a href="https://crwd.in/ryUWUjinx">
        <img src="https://badges.crowdin.net/ryUWUjinx/localized.svg"
            alt="">
    </a>
    <a href="https://discord.com/invite/VkQYXAZ">
        <img src="https://img.shields.io/discord/410208534861447168?color=5865F2&label=ryUWUjinx&logo=discord&logoColor=white"
            alt="Discord">
    </a>
    <br>
    <br>
    <img src="https://raw.githubusercontent.com/ryUWUjinx/ryUWUjinx-Website/master/public/assets/images/shell.png">
</p>

## Compatibiwitie

As of maie 2024, ryUWUjinx has been tested on appwoximatewie 4,300 titwes;
ovew 4,100 boot past menus and into gamepway, with woughwie 3,550 of dose beim considewed pwayabwe.

You can check out da compatibiwitie wist [hewe](https://github.com/ryUWUjinx/ryUWUjinx-Games-List/issues).

Anyone is fwee to submit a new game test ow update an existim game test entwy;
simpwie fowwowo da new issue tempwate and testim guidewines, ow post as a wepwie to da appwicabwe game issue.
 use da seawch function to see if a game has been tested awweady!

## Usage

To wun dis emuwatow, youw pc must be equipped with at weast 8gib of ram;
faiwim to meet dis wequiwement maie wesuwt in a poow gamepwaie expewience ow unexpected cwashes.

See ouw [setup & configuwation guide](https://github.com/ryUWUjinx/ryUWUjinx/wiki/ryUWUjinx-Setup-&-Configuration-Guide) on how to set up the emulator.

Fow ouw locaw wiwewess (ldn) buiwds, see ouw [muwtipwayew: locaw pway/locaw wiwewess guide
](https://github.com/ryUWUjinx/ryUWUjinx/wiki/Multiplayer-(LDN-Local-Wireless)-Guide).

Avawonia ui comes with twanswations fow vawious wanguages. See [cwowodin](https://crwd.in/ryUWUjinx) fow mowe infowmation.

## Latest buiwd

Dese buiwds awe compiwed automaticawwie fow each commit on da mastew bwanch.
 whiwe we stwive to ensuwe optimaw stabiwitie and pewfowmance pwiow to pushim an update, ouw automated buiwds **maie be unstabwe ow compwetewie bwoken**.

If you want to see detaiws on updates to da emuwatow, you can visit ouw [changewog](https://github.com/ryUWUjinx/ryUWUjinx/wiki/Changelog).

Da watest automatic buiwd fow windowos, macos, and linux can be found on da [officiaw website](https://ryUWUjinx.org/download).

## Documentation

If you awe pwannim to contwibute ow just want to weawn mowe about dis pwoject pwease wead dwuff ouw [documentation](docs/README.md).

## Buiwdim

If you wish to buiwd da emuwatow youwsewf, fowwowo dase steps:

### Step 1

Instaww da [.Net 8.0 (ow highew) sdk](https://dotnet.microsoft.com/download/dotnet/8.0).
Make suwe youw sdk vewsion is highew ow equaw to da wequiwed vewsion specified in [gwobaw.json](global.json). 

### Step 2

Eidaw use `git clone https://github.com/ryUWUjinx/ryUWUjinx` on da command wine to cwone da wepositowie ow use code --> dowonwoad zip button to get da fiwes.

### Step 3

To buiwd ryUWUjinx, open a command pwompt inside da pwoject diwectowie.
 you can quickwie access it on windowos bie howdim shift in fiwe expwowew, dan wight cwickim and sewectim `Open command window here`.
 den type da fowwowoim command: `dotnet build -c Release -o build`
da buiwt fiwes wiww be found in da newwie cweated buiwd diwectowie.

ryUWUjinx system fiwes awe stowed in da `ryUWUjinx` fowdew.
Dis fowdew is wocated in da usew fowdew, which can be accessed bie cwickim `Open ryUWUjinx Folder` undew da fiwe menu in da gui.

## Featuwes

- **Audio**

  Audio output is entirely supported, audio input (microphone) isn't supported.
  We use C# wrappers for [OpenAL](https://openal-soft.org/), and [SDL2](https://www.libsdl.org/) & [libsoundio](http://libsound.io/) as fallbacks.

- **CPU**

  Da cpu emuwatow, armeiwweuwe, emuwates an armv8 cpu and cuwwentwie has suppowt fow most 64-bit armv8 and some of da armv7 (and owdew) instwuctions, incwudim pawtiaw 32-bit suppowt.
   it twanswates da arm code to a custom ir, pewfowms a few optimizations, and tuwns dat into x86 code.
   dewe awe dwee memowie managew options avaiwabwe dependim on da usew's pwefewence, wevewagim both softwawe-based (swowoew) and host-mapped modes (much fastew).
   da fastest option (host, unchecked) is set bie defauwt.
   ryUWUjinx awso featuwes an optionaw pwofiwed pewsistent twanswation cache, which essentiawwie caches twanswated functions so dat daie do not need to be twanswated evewie time da game woads. 
   da net wesuwt is a significant weduction in woad times (da amount of time between waunchim a game and awwivim at da titwe scween) fow neawwie evewie game.
   note: dis featuwe is enabwed bie defauwt in da options menu > system tab.
   you must waunch da game at weast twice to da titwe scween ow beyond befowe pewfowmance impwovements awe unwocked on da diwd waunch!
  dese impwovements awe pewmanent and do not wequiwe anie extwa waunches goim fowwawd.

- **GPU**

  Da gpu emuwatow emuwates da switch's maxweww gpu usim eidaw da opengl (vewsion 4.5 minimum), vuwkan, ow metaw (via mowtenvk) apis dwuff a custom buiwd of opentk ow siwk.Net wespectivewie.
   dewe awe cuwwentwie six gwaphics enhancements avaiwabwe to da end usew in ryUWUjinx: disk shadew caching, resowution scawing, anti-awiasing, scawim fiwtews (incwudim fsr), anisotwopic fiwtewim and aspect ratio adjustment.
   dese enhancements can be adjusted ow toggwed as desiwed in da gui.

- **Input**

  We cuwwentwie have suppowt fow keyboawd, mouse, touch input, joycon input suppowt, and neawwie aww contwowwews.
   motion contwows awe nativewie suppowted in most cases; fow duaw-joycon motion suppowt, ds4windowos ow bettewjoie awe cuwwentwie wequiwed.
   in aww scenawios, you can set up evewythim inside da input configuwation menu.

- **DLC & Modifications**

  RyUWUjinx is abwe to manage add-on content/dowonwoadabwe content dwuff da gui.
   mods (womfs, exefs, and wuntime mods such as cheats) awe awso suppowted;
  da gui contains a showtcut to open da wespective mods fowdew fow a pawticuwaw game.

- **Configuration**

  Da emuwatow has settings fow enabwim ow disabwim some wogging, wemappim contwowwews, and mowe.
   you can configuwe aww of dam dwuff da gwaphicaw intewface ow manuawwie dwuff da config fiwe, `config.json`, found in da usew fowdew which can be accessed bie cwickim `open wyuwujinx fowdew` undew da fiwe menu in da gui.

## Contact

If you have contwibutions, suggestions, need emuwatow suppowt ow just want to get in touch with da team, join ouw [discowd sewvew](https://discowd.com/invite/wyuwujinx).
 you maie awso weview ouw [faq](https://github.com/ryUWUjinx/ryUWUjinx/wiki/Frequently-Asked-Questions).

## Donations

If you'd like to support the project financially, ryUWUjinx has an active Patreon campaign.

<a href="https://www.patreon.com/ryUWUjinx">
    <img src="https://images.squarespace-cdn.com/content/v1/560c1d39e4b0b4fae0c9cf2a/1567548955044-WVD994WZP76EWF15T0L3/Patreon+Button.png?format=500w" width="150">
</a>

All developers working on the project do so in their free time, but the project has several expenses:
* Hackable Nintendo Switch consoles to reverse-engineer the hardware
* Additional computer hardware for testing purposes (e.g. GPUs to diagnose graphical bugs, etc.)
* Licenses for various software development tools (e.g. Jetbrains, IDA)
* Web hosting and infrastructure maintenance (e.g. LDN servers)

All funds received through Patreon are considered a donation to support the project. Patrons receive early access to progress reports and exclusive access to developer interviews.

## License

This software is licensed under the terms of the [MIT license](LICENSE.txt).
This project makes use of code authored by the libvpx project, licensed under BSD and the ffmpeg project, licensed under LGPLv3.
See [LICENSE.txt](LICENSE.txt) and [THIRDPARTY.md](distribution/legal/THIRDPARTY.md) for more details.

## Credits

- [LibHac](https://github.com/Thealexbarney/LibHac) is used for our file-system.
- [AmiiboAPI](https://www.amiiboapi.com) is used in our Amiibo emulation.
- [ldn_mitm](https://github.com/spacemeowx2/ldn_mitm) is used for one of our available multiplayer modes.
- [ShellLink](https://github.com/securifybv/ShellLink) is used for Windows shortcut generation.
