Sample calibration data constants of ART radio test
=

Goal
-

All board revisions of every model of wireless devices should have at
least one sample here, though 2 or 3 samples would be preferred for
added redundancy.

This may sound excessive at first, but considering about 1KB/device,
the whole repository should not grow too large.

For simplicity of contribution, processing and restoration, the whole
64kB ART partition is saved, despite it being mostly empty.
git can compress it well.

Use
-

I would like to draw statistics of how a chipset behaves between
completely different devices, devices with only board revisions and
ones that are exactly the same.

Contributing
-

Please send a pull request to add your own sample to the collection.

Use the folder corresponding to the chipset of your wireless interface
card. You can find this at various sites online, such as:

  * https://www.wikidevi.com/
  * https://www.openwrt.org/
  * https://wiki.dd-wrt.com/wiki

To make the filename unique, it should contain:
  
  * the exact device model,
  * the exact model version and board revision,
  * the specific region code if printed (EU, HU, INTL, ...),
  * your name,
  * your MAC (or at least a few bytes from the end).

For example, the following is a valid filename:
  * `AR9331/TL-WR740N_v4.32_HU_bkil_11:22:33:44:55:66.bin`

Due to a lack of information, some existing files are missing board
revision. These samples will be deleted later on as better annotated
ones are gathered.

You should add metadata including references, contact, and site of
original publishing to your commit message.

License
-

To the extent possible under law, bkil has waived all copyright and
related or neighboring rights to calibrated-art-collection. This work
is published from: Hungary.

See the attached LICENSE file for terms. Original version:
https://creativecommons.org/share-your-work/public-domain/cc0/
https://en.wikipedia.org/wiki/CC0#Zero_/_public_domain

License rationale
-

Copyright protection does not apply to mathematical constants and other
data that is not considered creative work, including but not limited to
those calculated by algorithms or determined by machines without
creative human activities.

https://en.wikipedia.org/wiki/Copyright#Eligible_works

See also
-

* https://github.com/bkil/boot-loader-collection
