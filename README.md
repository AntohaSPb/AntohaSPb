- 👋 Hi, I am Anton
- 👀 I’m interested in AI image processing
- 🌱 I’m currently learning Python
- 💞️ I’m looking to collaborate on photo scans processing
- 📫 How to reach me - just whistle )
- 😄 Pronouns: Your majesty

This blog has been started to make available my scripts for processing of images being photos of printed pages.

Unlike normal scans made by household & office flatbed or sheet-fed scanners, pages that you have to photograph, e.g. in libraries, archives etc, suffer from three major issues making them unfit for immediate printed reproduction:

1. No uniform illumination causes edges beind too dark and image center being too bright. These under- and overexposed areas are called shadows and highlights. As such they are okay, but when treated together, mostly while rising global image contrast, textual information either in brighter or in darker areas gets erased or sinks in pixel noise. Extreme case of improper illumination is glare - direct, non-defused reflection of light from the scanned page into the camera sensor that totally blinds out a part of it, normally around 10%-15% of the page area.
   
2. Page geometry distortion caused by barrel effect of the camera lens and/or taking photo from a sharp angle. This may be easily corrected in Photoshop or GIMP by dragging the page corners, however as each page of the scanned document may have differing position of its corners, correcting everything manually or in batch mode is hardly a viable option.

3. Focus mismatch across center and edges of the photo. Common focusing algorythms of most smartphones and of digital cameras are tailored to taking normal photos, not scanning documents. Users may also not pay enough attention to select right scanning settings while digitizing printed material, and when focus issues are revealed, it may be too late to go re-digitizing the pages with defects. Images lightly blurred due to missed focus may be corrected, but if applied indiscriminatory, instead of slight defects in edges one gets extreme noise across the whole scanned page.   

There are other concerns, like differing white point levels across the multi-page document, different sizes of scanned pages that have the same actual printed size. To address these issues there should be a set of scripts inbetween scanning and collating scans into PDF, recognizing text, forms and images on the pages. Such scripts are available in ImageMagic batch processing package and other free software, however, with Python and image proocessing libraries you can build a custom solution that suits your needs best and integrates with furhter process of digitized documents' delivery. 

Employing AI is a revolutionary step in image processing. Instead of compiling a straight mathematical (images are about maths) algorythm and guessing the best parameters for your particular set of documents, you may 'teach' the neural network to create the result that you need from the source that you have. A common example of applied AI is image corners identification for further geometry correction.

Once I have a code snippet that more or less does the job, i put it here for my and community perusal. After all, everything I learned about AI, image processing and Python has been taken from the Git blogs, Youtube and other experience-sharing platforms across the Internet.

<!---
AntohaSPb/AntohaSPb is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
