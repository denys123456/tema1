# tema1 — Unity VR project

Unity Editor version: **6000.4.7f1**.

## Local setup

1. Obtain Vuforia Engine **11.4.4** from its official distribution and place
   `com.ptc.vuforia.engine-11.4.4.tgz` in `Packages/` before opening Unity.
   Both package manifests intentionally reference this local archive.
   The archive is excluded from Git; this repository does not use Git LFS.
2. Open the project with the matching Unity Editor version.
3. Configure your own Vuforia license locally. The committed
   `Assets/Resources/VuforiaConfiguration.asset` has empty license fields.
   Never stage license values; clear both `vuforiaLicenseKey` and
   `ufoLicenseKey` before committing changes to that asset.

On the original workstation, the previous Vuforia configuration is backed up
in the ignored `.secrets/VuforiaConfiguration.asset`. Do not publish it.

The Chicken Warrior FBX is used by `Assets/OutdoorsScene.unity` and is tracked.
Unity-generated folders and the local `QCAR/lh` and `QCAR/somedata16` files
are excluded from version control.
