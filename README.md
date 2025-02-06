# Hoodoo GPU architecture custom campaign

This is the repository containing levels of the custom campaign for the game [Turing Complete](https://store.steampowered.com/app/1444480/Turing_Complete/).

## Features

- Introduction to signed fixed-point numbers
- Explaining the basics of rasterization, including color interpolation and barycentric coordinates
- Build a GPU capable of rendering 3D models

## Installation Instructions

First of all, you need to download the campaign:
1. Download one of the releases on the right side
2. Unpack the contents (You should get a bunch of folders starting with `gpu_`)
3. Move the folders into the level directory in your Turing Complete game files
4. Start the game

Then you have three ways to play the campaign:
1. In the main menu, press `Q` and in the console type `load gpu_campaign`, and press `Enter`.
That will load the campaign screen.
Unfortunately with this approach you have to load the campaign screen again after completing each level.

2. Using `dev_mode` you can add the `gpu_campaign` level to the main campaign screen.
That makes it much easier to open the campaign each time you complete a level.

3. Using `dev_mode` you can add all the levels of the campaign to the main campaign screen.
This approach is the most work, but after completing a level you are moved back directly to the campaign.

## Preview

![](images/1.png)

![](images/2.png)

![](images/3.png)

## Roadmap

Legend:  
:heavy_check_mark: - Done  
:hammer: - In Progress  
:o: - Not Done Yet  
:x: - Probably won't be supported

- V1:
    - :heavy_check_mark: Fixed-point numbers introduction
    - :heavy_check_mark: Basics of triangle processing - interpolation, barycentric coordinates
    - :heavy_check_mark: Vector and Matrix operations
    - :hammer: Setting up the MVP matrix and projecting vertices
    - :hammer: Decoding five simple commands (draw, get_status, change_ram_offset, change_triangle_count, change_mvp)
    - :hammer: Getting the rasterizer and vertex transformer together into `Hoodoo V1`
- V2:
    - :o: Half-pixel correction
    - :o: Alpha composition
    - :o: Backface culling
    - :o: Hardware dithering
    - :o: Double buffering
    - :o: Z-buffer
    - :o: More rasterizers in parallel
    - :o: Fully programmable pipeline

## Contributing

If you want to contribute to the campaign, feel free to report bugs, make feature requests and send PRs!

**Enjoy!**