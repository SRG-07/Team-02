# Team-02
DECENTRALISED SECURE STORAGE SYSTEM

Task-01:
1) First i installed the Pillow library which is used for image loading,editing and saving
2) I downloaded the image from net and uploaded it in my colab and opened it in my .ipynb file using PIL(pillow)
3) Then i gave the secret message and converted it into bits(binary form)
4) Now i stored the values of RBG (red,green,blue) in pixels from the image
5) I have encoded my message only in the red channel by clearing the last bit of red and replacing it with 0 or 1 based on the message
6) This reults in new list of pixel that looks identical to the original to human eye
7) Then stored the encoded_image
8) While decode it i took the red value and extracted the least significant bit(or last digit of 8 bit binary) and grouped every 8 bits and converted them back to character
9) Finaly displaced the encoded message

I chose Least Significant Bit method as it is simple and the output image has no visual changes. Other method such as DCT(Discrete Cosine Transform) which hides data in frequnce domain by modifying DCT coefficients and is more Complex and slower, and DWT (Discrete Wavelet Transform) which hides data in the wavelet transformed image(across different resolution levels) and is harder to implement. It’s perfect for understanding the core concept of hiding information in digital images before exploring more advanced (and secure) methods like DCT or DWT. I haven't gone in depth about these two methods yet.
