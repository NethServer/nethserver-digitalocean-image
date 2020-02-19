# Nethserver DigitalOcean image generator

Generate a base Nethserver image that can be used for create new droplets.

For using the images in the DigitalOcean cloud platform, you have to upload it as
[Custom Image](https://www.digitalocean.com/docs/images/custom-images/how-to/upload/).
A list of ready to use images can be found in the Releases page.

**WARNING the default credentials are: `root`/`Nethesis,1234`**

## Build requirements

* [packer.io](https://packer.io/)

## Build

* Build new image:
  * Nethserver Community: `packer.io build nethserver.json`
  * Nethserver Enterprise: `packer.io build nethserver-enterprise.json`

After the creation you can find the generated `qcow2` images in the `output_qemu` directory.
