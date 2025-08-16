# PReloader
A patched version of the closed-source [PreLoader](https://github.com/LiteLDev/Preloader), deobfuscated with some restrictions removed.

> [!TIP]
> The patch contents may vary in different versions. Please read the release notes.

## Notes
 - This is a patch directly on the original binary DLL, so no guarantees can be given, it should work as is.
 - If you encounter crashes, please file an issue or chat with us in the community.

## Usage

#### For developers
 - Use PReloader to replace PreLoader, just add the repository in `xmake.lua`:
```lua
add_repository("liteldev-free-repo https://github.com/liteldev-free/xmake-repo.git")

-- If you haven't imported the package yet...
add_requires("preloader")

-- Use it in your project....
target("YourProj")
    add_packages("preloader")
```

#### For reverse engineers
 - If IDA can't disassemble or identify a function correctly, [Igor's tip](https://hex-rays.com/blog/igors-tip-of-the-week-152-force-creating-functions) is your friend.

#### For regular users
 - Just replace `PreLoader.dll`.

## Community

Our vision is to build an open and inclusive Minecraft: Bedrock Edition ecosystem.

- [Discord](https://discord.gg/fPKVZScPT7)
- [Telegram (Channel)](https://t.me/s/bdsplugins)
