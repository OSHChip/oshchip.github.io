---
layout: page
title: Hello from OSHChip
excerpt: "Hello page"
tags: [nRF51822, BLE]
categories: [Electronics]
comments: true
modified: 2015-12-26

thumbnail: images/2015/10/oshchip.jpg
image:
  feature: header.jpg
---

# Heading 1

## Heading 1

### Heading 3

List:

* nRF51822
* BLE
* OSHChip

Numbered list:

1. nRF51822
2. BLE
3. OSHChip

Some code:

{% highlight sh %}
{% raw %}
/* Linker script to configure memory regions. */

SEARCH_DIR(.)
GROUP(-lgcc -lc -lnosys)

MEMORY
{
  FLASH (rx) : ORIGIN = 0x18000, LENGTH = 0x28000
  RAM (rwx) :  ORIGIN = 0x20002000, LENGTH = 0x2000
}

INCLUDE "gcc_nrf51_common.ld"
{% endraw %}
{% endhighlight %}


An image:

![OSHChip](/images/2015/10/oshchip2.png "OSHChip")


Here's a sample table:

| nRF51-DK | RBL Nano |
|:--------:|:--------:|
| SH_VTG  | VDD |
| SH_SWDIO | SWDIO |
| SH_SWDCLK | SWCLK |
| SH GND DETECT | GND |
| GND | GND |

This is a [link][1].

Here's some math - uses LaTeX syntax.

$$e^\pi + 1 = 0$$

Here's an embedded video:

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/pIaPSRHiDrM" frameborder="0" allowfullscreen></iframe>
</p>


[1]: https://hackaday.io/project/7212-oshchip-v10



