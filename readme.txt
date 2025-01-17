Read Me
This is a script about creating a Jazz poster in GIMP.

A variable named jazz_poster is defined in the script, which has 14 parameters.
jazz_poster(file1, file2, file3, file4, file5, str1, font1, str2, font2, str3, font3, radius, amount, value)

The size of the poster is A4 composition, so set the width and height of poster are 2480px and 3508px.

There are five images used in this poster.
1. image1.jpeg
2. image2.png
3. image3.png
4. image4.png
5. image5.png

Design principles:
1. Balance
The overall poster is a symmetrical layout. 
The positions of image2 and image3 are symmetrical. The musician playing the saxophone in image2 and the beating notes in image3 together form a harmonious picture.

2. Proximity and Alignment
The poster title is located on the central axis of the poster, with the same left and right margins.
Almost all elements on the poster have a certain margin.

3. Unity
The pictures on the poster are all musicians and jazz instruments related to jazz themes.
image4 is a geometric figure composed of different fan shapes mainly in blue and pink colors.
The text color is the same as the main color in image4.
The surrounding circle fills the blank of the poster, making the poster look more complete.

4. Emphasis
The main function of image4 is to emphasize the title of the poster.
The title color of the poster is black, which happens to have a strong contrast with the blue and pink of image4, which is more attractive to people’s attention.
In addition, adding a drop-shadow effect to the title of the poster to make the title more layered.

5. Rhythm
image2 and image3 have a feeling of musicians playing beautiful notes with a saxophone, which adds rhythm and vividness to the poster.

Personal Contributions:
1. Image1 as the background image of poster is used a HSV Noise effect to increase the graininess.
    pdb. plug_in_hsv_noise(image1, layer1, 2, 3, 0.5, value)
    The value can be changed by adjusting the slider.

2. Using the unsharp mask filter to process image2, so that the color of image2 is no longer completely black, increasing the sense of three-dimensionality and gloss.
    pdb.plug_in_unsharp_mask(image2, layer2, radius, amount, 0)
    The radius and amount can be changed by adjusting the slider.

3. Setting a drop-shadow effect for the title to add three-dimensionality and layering.
    pdb.script_fu_drop_shadow(posterImage, textLayer1, 20, 20, 10, (0, 0, 0), 50, False)

4. In addition to the poster title, two text boxes are also set up to fill in the blanks of the poster. 
    These two texts are slogans about jazz, which adopt different fonts and font colors to prevents the posters from being boring.