---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: MOV
---

<table>
  <tr>
    <td> <img style="float: left" class="ui image" src="../../images/mov-timeline.jpg"> </td>
    <td> <img style="float: left" class="ui image" src="../../images/mov-video-edit.png"> </td>
    <td> <img style="float: left" class="ui image" src="../../images/mov-video-view.png"> </td>
  </tr>
</table> <br>

Mov is a Swift-based iOS app that provides a mobile-oriented interface for video editing using Apple’s built-in [AV Foundation](https://developer.apple.com/av-foundation/) framework. The app was a collaboration between myself and a friend for his Computer Engineering capstone project at UH Manoa.

## Design

Mov is designed around representing video clips in a vertical, card-based timeline. Clips can be trimmed and rearranged along the timeline like a physical stack of cards, and the final video would be exported in the order of the stack.

## Program Structure

The app was designed programmatically, mostly within a primary View Controller handling the timeline interface as well as the core functions for importing and merging videos, and an additional View Controller for trimming individual clips.

The timeline was written by extending both [UICollectionView](https://developer.apple.com/documentation/uikit/uicollectionview) and [UICollectionViewCell](https://developer.apple.com/documentation/uikit/uicollectionviewcell). The videos were maintained using a simple array, rearranging the indices whenever any movement for the corresponding cells was handled.

The [Hero](https://github.com/lkzhao/Hero) framework was implemented to provide fluid animations.

## Contributions

I contributed to the project in both design and implementation. Since it was both mine and my friend’s first experience working with most of the frameworks used, much of the coding and debugging was performed in over-the-shoulder collaboration. We both were involved in the implementation of the CollectionView timeline and video editing functionality.

## Takeaways
Mov was exposed me to 100% code-based mobile development, as well as experience in implementing frameworks in iOS. Additionally, it forced me to think critically about designing a traditionally-desktop experience around the constraints of a mobile environment. One of the biggest challenges was working in a suboptimal environment-- I didn't have a Macbook available, so I had to set up a macOS VM through [VirtualBox](https://www.virtualbox.org/wiki/VirtualBox).
