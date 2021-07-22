---
title: Creating An Artboard in Sketch
_description: How to Sketch Artboard for a registration screen using Indigo Design Libraries.
_keywords: Design Systems, Design Systems UX, UI kit, Sketch, Ignite UI for Angular, Sketch to Angular, Angular, Angular Design System, Export code from Sketch, Design Kits for Angular, Sketch HTML, Sketch to HTML, Sketch UI kits
---

# Creating Your First Artboard in Sketch

At the end of this topic you'll have a Sketch Artboard for a registration screen using the **Indigo.Design System**. If you use Adobe XD for design then jump to [this topic](creating-artboard-adobexd.md).

<div class="divider--half"></div>
<img class="responsive-img" src="images/getting-started-sketch7.png" srcset="images/getting-started-sketch7@2x.png 2x" />
<div class="divider--half"></div>
<div class="divider--half"></div>
<div class="divider--half"></div>
<div class="divider--half"></div>
<div class="divider--half"></div>

## What you need

If the [Titillium Web Font][1] isn't installed on your computer, please do it before starting. All texts in the **Indigo.Design System** use it.

## Step by step

### 1. Add the **Indigo.Design System** as a Library.

1.  Download the [**Indigo.Design System**](https://cloud.indigo.design/home).

    It contains a Sketch file with 26 Pages in the Pages section which are distinguished by three types of icons:

    - **🎨 ~** styling pages: all the styling assets such as Material Icons, Colors, Typography, Elevation, and Illustrations can be found in the five pages on top.

    - **🧩 Components**  page: a vast set of Components to layout your design ideas.
      Through various presets available in the `Insert` menu and overrides for states and layouts to configure in the right panel of the Sketch UI, you can create layouts compatible with Ignite UI for Angular and our code generation engine.

    - **🌆 ~** patterns pages: the components shape up meaningful patterns for productive application design that can be found spread across the remaining pages.

2.  Open up the Sketch app on your Mac, click on the Sketch in the App Menu, and select Preferences.

3.  In the dialog, select the `Libraries` tab and click the **Add Library...** button.

4.  Navigate to the folder where you have downloaded the library.

5.  Select it and click `Open`.

6.  Make sure it shows up in the list in the `Preferences` dialog and that it is checked.

  <div class="divider--half"></div>
  <img class="responsive-img" src="images/Creating_An_Artboard_Sketch2.png" srcset="images/Creating_An_Artboard_Sketch2@2x.png 2x" />
  <div class="divider--half"></div>
  <div class="divider--half"></div>
  <div class="divider--half"></div>
  <div class="divider--half"></div>
  <div class="divider--half"></div>

You may have noticed that in the image above, the library also appears to be present in my Sketch cloud, and as an alternative, you can use this mechanism if you are running version 57 or later. The set up is very easy, you only need to open the Indigo.Design Sketch file and save it in your Sketch cloud. A detailed explanation of how to set Indigo.Design as a cloud library can be found in [this Medium post](https://medium.com/ignite-ui/using-indigo-design-with-sketch-cloud-libraries-70533bca00f8). Once you added the library successfully, it will show up in the `Symbols` section of the `Insert` menu.

> [!Note]
> If you already have the **Indigo.Design System** set up in Sketch and want upgrade to a newer version, open your Sketch preferences, delete the current library and install the new one following the steps above. Make sure to reapply any themes and customizations via the [Indigo.Design plugin](sync-themes-plugin.md) and note that you may have to link some components or overrides in your design files manually to the symbols in the new library if Sketch does not do that automatically for you.

### 2. Create an artboard.

1.  In the Sketch app on your Mac, create a new file.
2.  Select the Artboard size.  
    Press the `A` key and select the artboard size from the panel on the right.  
    This example is for an iPhone 11 in portrait orientation (414x896). If you don't see this preset artboard, choose Apple Devices from the dropdown at the top of the panel.

  <div class="divider--half"></div>
  <img class="responsive-img" src="images/getting-started-sketch-artboard.png" srcset="images/getting-started-sketch-artboard@2x.png 2x" />
  <div class="divider--half"></div>
  <div class="divider--half"></div>
  <div class="divider--half"></div>
  <div class="divider--half"></div>
  <div class="divider--half"></div>

### 3. Add and customize components.

We will use the `Insert` menu to add components from the Indigo Design Library, and then customize them using the panel on the right.

These are the steps to recreate the screen in the example.

1.  **Add the Navbar.**

    1.  From the `Insert` menu, select Symbols / Indigo.Design / Navigation / Navbar / Elevated.
    2.  Place it at the top of the artboard and stretch it to take up all the width available.
    3.  In the Resizing section of the panel on the right, pin it to the top of the artboard and fix its height.
    4.  In the Overrides section, set the Left Action to ~No Symbol, then set the Title to "Sign Up". After that set the 1 | Icon, 2 | Icon, and 3 | Icon to ~No Symbol.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch0.png" srcset="images/getting-started-sketch0@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

2.  **Add the background color.**  
     Press the `R` key and drag а rectangular shape, making sure it's sized accordingly to fill the available area below the Navbar and is also under it as a layer. With the rectangle selected, in the right panel under Appearance you will find a Layer Style dropdown. Open it and choose Indigo.Design / Color / Fill / primary.100.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch1.png" srcset="images/getting-started-sketch1@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

3.  **Add the background for the form.**

    1.  Press the `R` key again and drag а rectangular shape with size 280x378.
    2.  Assign the following style to it Indigo.Design / Color / Fill / white.
    3.  Position it in the center of the artboard.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch2.png" srcset="images/getting-started-sketch2@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

4.  **Add the title of the form.**

    1.  Press the `T` key to add a text element on top of the white rectangle and type "Start Budgeting" in it.
    2.  Assign the following typography style to it similarly to how a color was assigned to a rectangle above but under Appearance you will find a Text Style dropdown. Open it and choose Indigo.Design / H4 Headline / Center / Active.
    3.  Place it at the top of the white rectangle, with 16px spacing on the top.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch3.png" srcset="images/getting-started-sketch3@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

5.  **Add the inputs for first and last name.**

    1.  From the `Insert` menu, select Symbols / Indigo.Design / Input / Simple / Line / Enabled.
    2.  In the Overrides section, set the State to ~Filled.
    3.  Set the Prefix Container and the Suffix Container to ~No Symbol.
    4.  Set the Label to "First Name", and the Value to "Eliza".
    5.  Place it below the title. Leave 16px on the left and top.
    6.  Set its width to 116px.
    7.  Duplicate this input.
    8.  Place the new one to the right of the first one, with 16px spacing between the two.
    9.  In the Overrides section, set the Label to "Last Name", and the Value to "Morales".

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch4.png" srcset="images/getting-started-sketch4@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

6.  **Add the inputs for user name and password.**

    1.  Duplicate one of the Name inputs twice to create two more inputs for Username and Password.
    2.  Place them one under the other with a vertical spacing of 16px between each other and to the ones from the previous step.
    3.  Stretch them across the full width with 16px spacing on both sides.
    4.  In the Overrides section, set their Labels to "Username" and "Password" and their Values to "Leaellynasaura" and "\*\*\*\*\*\*\*\*\*\*\*\*".
    5.  While there also set the Password input's Content Type to Password.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch5.png" srcset="images/getting-started-sketch5@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

7.  **Add the sign up button.**

    1.  From the `Insert` menu, select Symbols / Indigo.Design / Button / Raised / Enabled.
    2.  Place it below the inputs, stretch it across the full width leaving 16px on the left, right, and from the inputs above.
    3.  In the Overrides section, set the Before Icon and the After Icon to ~No Symbol.
    4. Set the Text to "SIGN UP" and update its Style to ~White.
    5. Update the Background to ~info.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch6.png" srcset="images/getting-started-sketch6@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

8.  **Add the terms acceptance text.**

    1.  Press the `T` key to add another text element below the button and type "By clicking on the "SIGN UP" button above, you accept our Terms of Use" in it.
    2.  Assign the following Style to it Indigo.Design / Caption / Center / Inactive.
    3.  Change its size so that there is a 16px spacing on the left, right and above.

    <div class="divider--half"></div>
    <img class="responsive-img" src="images/getting-started-sketch7.png" srcset="images/getting-started-sketch7@2x.png 2x" />
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>
    <div class="divider--half"></div>

9.  **Make the artboard responsive.**

    1.  Select the text layers, inputs, button and white rectangle, and group them.
    2.  Fix the width and height of the group and pin it to the top from the Resizing options in the panel on the right.

## Additional Resources

Related topics:

- [Creating Your First Artboard in Adobe XD](creating-artboard-adobexd.md)
- [Button](components/button.md)
- [Input](components/input.md)
- [Navbar](components/navbar.md)
- [Text](components/text.md)
- [Styling](style/styling-overview.md)
  <div class="divider--half"></div>

Our community is active and always welcoming to new ideas.



[1]: https://fonts.google.com/specimen/Titillium+Web
