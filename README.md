# VRLog Updates

This public repository contains only signed update metadata and binary delta packages for an already installed copy of VRLog.

公開しているのは、インストール済みVRLogを更新するための署名済みフィードと差分パッケージだけです。初回インストールに必要な完全なSetup EXE、完全パッケージ、VRLog.exe、DLL、ポータブル版、ソースコードは含みません。

## Files

- `releases.win.json`: signed release metadata
- `releases.win.json.sig`: Minisign-compatible signature for the metadata
- `*-delta.nupkg`: binary changes that require the matching installed base version

The delta files are not standalone applications and cannot install or launch VRLog without the matching base product. Public availability does not grant a license to redistribute, reverse engineer, modify, sublicense, or create a competing product. VRLog's EULA and each third-party component's own license continue to apply.

差分単体はアプリではなく、対応する完全版がなければインストールも起動もできません。この公開はVRLog本体の再配布、解析、改変、再許諾、競合製品への利用を許可するものではありません。VRLogのEULAと第三者コンポーネント固有のライセンスが適用されます。

The embedded VRLog public key verifies the feed before any delta is accepted. This signature verifies update origin and integrity; it is not purchaser authentication or DRM.

VRLogは内蔵公開鍵でフィードを検証してから差分を受け入れます。この署名は更新の発行元と改ざんを確認するもので、購入者認証や完全なDRMではありません。

Copyright (C) 2026 YUMA. All rights reserved, except for separately identified third-party components.
