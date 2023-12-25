# Meta-Debian-Package for the Pinenote kernels

Based on the example definition helpfully provided by Jonas Smedegaard:

https://salsa.debian.org/tinker-team/linux-pinenote

This packages generates four metapackages:

	* linux-image-pinenote-stable
	* linux-headers-pinenote-stable
	* linux-image-pinenote-testing
	* linux-headers-pinenote-testing

## Generating the packages:

	gpb clone [URL]; cd linux-pinenote; gbp buildpackage --git-no-sign-tags

* Increase a new version of the meta packages

	dch -i; gbp dch --release
