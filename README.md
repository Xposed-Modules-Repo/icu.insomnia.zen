<div align="center">


<h1>ZEN</h1>

> 

<div align="center">


  [![Stars](https://img.shields.io/github/stars/Xposed-Modules-Repo/icu.insomnia.zen?label=stars)](https://github.com/Xposed-Modules-Repo/icu.insomnia.zen)
  [![LSP%20Repo](https://img.shields.io/github/downloads/Xposed-Modules-Repo/icu.insomnia.zen/total?label=LSP%20Repo&labelColor=F48FB1)](https://github.com/Xposed-Modules-Repo/icu.insomnia.zen/releases)
</div>

[![Release](https://img.shields.io/github/v/release/Xposed-Modules-Repo/icu.insomnia.zen)](https://github.com/Xposed-Modules-Repo/icu.insomnia.zen/releases/latest)

</div>




# Warning

Make sure you are able to recover device when anything unexpected take place!

Make sure you are able to recover device when anything unexpected take place!

Make sure you are able to recover device when anything unexpected take place!

# Basical Usage

1. Install the `release.apk` directly
2. Activate NightGuard, and check the target apps in Lsp manager
3. Adding time-spans in NightGuard to set the sleep time


## Enhance：

NightGuard is based on Lsposed, and an alternative enhanced with Magisk. So there 2 enhanced way for user.


1. Still install directly

   1. Disable Lsp continuing notification and remove the Lsp manager shortcut.
   2. Check the **app-installer** of you system in Lsp manager. (When new xposed app installed, a Notification will be sent by Lsp manager)
   3. Check the **tell-dial** of you system in Lsp manager, which is different from the **incall-app**. You are able to handle in call but could not dial if you check. (Some special code can invoke the Lsp manager)
   4. Check any File-Manager that has the root access. (Prevent remove NightGuard in File-Manager)
2. Use magisk to install

   1. You can install the magisk module in release list, which help install NightGuard as system app. (Un-uninstallable)
   2. Remove Magisk manager, which dose not lose your root and could be reinstalled anytime. (Prevent Magisk module be disabled)
   3. Check any File-Manager that has the root access. (Prevent remove Magisk module in File-Manager)
  
