# grub-themes

My pack of GRUB2 themes for different Linux distributions and It aims to replace the default GRUB look, with a nice and colorful theme.

## About

This project is based on [distro-grub-themes](https://github.com/AdisonCavani/distro-grub-themes), a GPLv3-licensed software.

## Usage

### 1. Clone this repo

```bash
git clone https://github.com/rolodoom/grub-themes
```

### 2. Copy theme

Just copy the desire theme from the `themes` folder to `/boot/grub/themes/` and add

```bash
sudo cp -r grub-themes/themes/{theme-name} /boot/grub/themes
```

> Remember to change `{theme-name}` for the theme you want to use.

### 3. Enable theme

Add the following string to the `/etc/default/grub` file.

> Remember to change `{theme-name}` for the theme you want to use.

```bash
GRUB_THEME="/boot/grub/themes/{theme-name}/theme.txt"
```

### 4. Update grub

Run the following command to update the changes into the grub.

```bash
sudo update-grub
```

## Troubleshoting

Don't forget to delete or rename the default theme as sometimes you don't see the change and it is because programmatically it is loading the theme that the distro installed by default in `/boot/grub/themes/`.

## Bugs and Issues

Have a bug or an issue with this themes? [Open a new issue](https://github.com/rolodoom/grub-themes/issues) here on GitHub.

## License

This code is released under the [GPLv3](https://github.com/rolodoom/grub-themes/blob/master/LICENSE) license, which means you have the four freedoms to run, study, share, and modify the software. Any derivative work must be distributed under the same or equivalent license terms.
