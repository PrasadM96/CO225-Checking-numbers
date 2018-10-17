CO225-Checking-numbers
When doing any work with visual media it is often very useful to have the complement of a
color on hand to create contrast and bring the focus of a picture to a particular place. To create
the complement of a color on a computer, each of the red, green, and blue values of a color are
inverted. Each of the red, green, and blue values of a color can range from 0 to 255, inclusive. If a
particular component of one color is 50, then that component of its complement is 255-50=205.
Although this generally works well, it doesnt generate good complements for grey colors that
have all three components right around 128. To x this you will return an alternate complement for
grey colors. If each component of a color and its corresponding component of the colors comple-
ment dier by 32 or less, then make the complement of each component by either adding 128 to a
components value, or by subtracting 128 from a components value, whichever one results in a legal
value. For example, the color 115,115,143 would have the complement 140, 140,112, but since
each component of the complement would have been within 32 of the corresponding component of
rgb, we return the alternate complement 243, 243, 15 instead.
