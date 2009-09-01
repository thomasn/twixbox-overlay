# twixbox-overlay

Assorted ebuilds for Gentoo Portage that haven't made it to 'sunrise' yet.

## Contents

Available ebuilds:

 * clamz - a commandline Amazon MP3 downloader, as an alternative to net-misc/amazonmp3
   - ebuild from http://bugs.gentoo.org/267873

## Installation

As root:

    emerge -av layman
    $EDITOR /etc/layman/layman.cfg    # Add to 'overlays' section:
      http://github.com/thomasn/twixbox-overlay/blob/master/overlay.xml?raw=true
    layman -L
    layman -a twixbox-overlay
    layman -S
    layman -l    # should show 'twixbox-overlay'
    echo 'source /usr/portage/local/layman/make.conf' >> /etc/make.conf
    emerge -av net-misc/clamz

Feedback via github please.
