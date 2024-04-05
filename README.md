**<u>ASSIGNMENT REPORT - APPLICATION</u>**

**<u>1. PURPOSE OF THE APP</u>**

The purpose of this application is to garner educational technology and
its growth.

And the person who will be using the app is Sarah, a close family member
asked me if I could build an application. She is a history and a teacher
who wants to use innovative technology.

She requests an application where a user inputs an age and that will
generate a historical figure who passed on at that age.

**<u>2. Design Considerations</u>**

<u>**Intuitive Design**:</u>

My application where you can type the age of the person that died and
where the main generate button is located at the bottom of the screen,
allowing users to easily access key features with their thumbs.

<u>**Content Prioritization**:</u>

My app that prominently displays the featured pictures at the top of the
homepage, and at the bottom is the action buttons that will generate
what you will be looking for when you type in an age

<u>**Legible Text Content**:</u>

On my app every word is readable, and you can see it clearly cause I
used a system-Ui font which is very readable and visible and enlarged
the font size to 24dp which is for simple reading

<u>**Make Interface Elements Clearly Visible**:</u>

On my app with distinct icons for different actions spaced apart with
enough padding to avoid confusion and clear labels for each element so
you can see and avoid overcrowding things.

<u>**Hand Position Controls**:</u>

On my app the action buttons are positioned near the bottom corners of
the screen, allowing the users to easily reach them with their thumbs
while holding the device.

**<u>IMAGES</u>**

The reason I chose that picture was because it provides immediate visual
context to users setting the tone for the content and subject matter of
the app and it helps users to understand what the app is about at first
glance making it more visually appealing and memorable for users

And the reason it is at the top of the interface is because the top of
the interface is the first thing users see when they open the app, and
it ensures that it is the first thing the users notice when they open
the app making a strong first impression and immediately communicating
the app's purpose.

**3. <u>GITHUB AND GITHUB ACTIONS</u>**

[<u>https://github.com/st10460324/MyApp</u>](https://github.com/st10460324/MyApp)

**<u>1. Create a New GitHub Repository:</u>**

-   Go to the GitHub website
    > ([<u>https://github.com/</u>](https://github.com/)) and sign in to
    > your account.

-   Click on the "+" icon in the top right corner and select "New
    > repository".

-   Give your repository a name (your student number and name – in one
    > word), add a description (use IMAD5112 Assignment 1) and choose
    > public.

-   Click on the "Create repository" button.

**<u>2. Initialise the Repository with a README File</u>:**

-   After creating the repository, you'll see an option to "Initialize
    > this repository with a README". Check this option to create a
    > README file.

-   Click on the "Create repository" button to finalize the creation of
    > the repository.

**<u>3. Commit and Push Your Project Files to the GitHub
Repository:</u>**

-   In Android Studio, go to VCS (Version Control System) -> Import into
    > Version Control -> Share Project on GitHub.

-   Log in to your GitHub account if prompted, and select the repository
    > you created earlier.

-   Click on the "Share" button to push your project files to the GitHub
    > repository.

**<u>4. Regularly Commit and Push Your Code as You Make Progress:</u>**

-   After the initial push, continue making changes to your project in
    > Android Studio.

-   Whenever you make significant progress or changes, commit your
    > changes locally in Android Studio using VCS -> Commit Changes.

-   Once committed, push your changes to the GitHub repository using VCS
    > ->Git -> Push.

-   Testing and Automated Testing:

**<u>1. Conduct Manual Testing</u>:**

-   Manually test your app to ensure it functions seamlessly and offers
    > an enjoyable educational experience for learners.

-   To test various features and user interactions do the following:

**<u>1. Create a New Test Class</u>:**

-   In your Android project, navigate to the tests directory (or create
    > it if it doesn't exist).

-   Create a new Kotlin file for your test class. Name it appropriately
    > to indicate what component or functionality you are testing.

**<u>2. Write Test Methods</u>:**

-   Inside the test class, write test methods like the example below.

**<u>3. Use assertions to verify the expected behaviour of your
code.</u>**

**<u>4. Run the Tests</u>:**

-   Run the tests using the testing framework's tools provided by
    > Android Studio or through the command line.

Sample of a test class using JUnit:

import org.junit.Assert.\*

import org.junit.Test

class MyUnitTest {

@Test

fun testWhenStatement() {

// Test case for a when statement

val result = when (25) {

95 -> "Nelson Mandela, famous for …, died at this age" // your own
wording (copy from your code) – only need 3 ages from your code for the
test here.

30 -> "steve biko, famous for ……., died at this age"

25 -> "tupac, famous for …..., died at this age"

else -> "Nobody famous known to me died at this age"

}

assertEquals("Nobody famous known to me died at this age", result)

}

}

**<u>2. GitHub Actions for Automated Testing</u>**:

-   Set up GitHub Actions to automatically run tests and build your code
    > whenever changes are pushed to the repository.

-   Create a GitHub Actions workflow (.github/workflows/tests.yml) to
    > run tests automatically on every push:

-   Create a .github/workflows directory in your project repository.

-   Inside this directory, create YAML files defining your GitHub
    > Actions workflows for testing and building.

Sample GitHub Actions Workflow for Testing (tests.yml):

name: Run Tests

on: \[push\]

jobs:

test:

runs-on: ubuntu-latest

steps:

\- name: Set up JDK

uses: actions/setup-java@v2

with:

distribution: 'adopt'

java-version: '11'

\- name: Check out code

uses: actions/checkout@v2

\- name: Build and test

run: ./gradlew test

Set Up Automated Build:

Create a GitHub Actions workflow (.github/workflows/build.yml) to build
the APK automatically on every push.

Sample GitHub Actions Workflow for Building (build.yml):

name: Build APK

on: \[push\]

jobs:

build:

runs-on: ubuntu-latest

steps:

\- name: Set up JDK

uses: actions/setup-java@v2

with:

distribution: 'adopt'

java-version: '11'

\- name: Check out code

uses: actions/checkout@v2

\- name: Build APK

run: ./gradlew assembleDebug

Test your workflows by pushing changes to your repository and observing
the actions running in the "Actions" tab on GitHub.

**4. <u>LINK TO YOUTUBE VIDEO</u>**

[<u>https://eur03.safelinks.protection.outlook.com/?url=https%3A%2F%2Fyoutu.be%2FCs179lXRtUs%3Fsi%3D5sn6dJ67dAE7urE6&data=05%7C02%7CSt10460324%40vcconnect.edu.za%7Ca7fc5f18712e47ded56608dc556c54d2%7Ce10c8f44f469448fbc0dd781288ff01b%7C0%7C0%7C638479170991354953%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=I%2BiU7c6lcXZCX%2BiaBCppYD%2BcB0lpqFRYQeeU8z8wmII%3D&reserved=0</u>](https://eur03.safelinks.protection.outlook.com/?url=https%3A%2F%2Fyoutu.be%2FCs179lXRtUs%3Fsi%3D5sn6dJ67dAE7urE6&data=05%7C02%7CSt10460324%40vcconnect.edu.za%7Ca7fc5f18712e47ded56608dc556c54d2%7Ce10c8f44f469448fbc0dd781288ff01b%7C0%7C0%7C638479170991354953%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=I%2BiU7c6lcXZCX%2BiaBCppYD%2BcB0lpqFRYQeeU8z8wmII%3D&reserved=0)

**5. <u>REFERENCE LIST</u>**

-   Wikipedia. (2023). *Nelson Mandela*. \[online\] Available at:
    > [<u>https://en.wikipedia.org/wiki/Nelson_Mandela#CITEREFSampson2011</u>](https://en.wikipedia.org/wiki/Nelson_Mandela)

-   Samuels, A.J. (2012). *Bob Marley: Anatomy of an Icon*. \[online\]
    > Culture Trip. Available at:
    > [<u>https://theculturetrip.com/caribbean/jamaica/articles/bob-marley-anatomy-of-an-icon/</u>](https://theculturetrip.com/caribbean/jamaica/articles/bob-marley-anatomy-of-an-icon/).

‌

-   actbox: The life and death of pop star Michael Jackson. (2011).
    > *Reuters*. \[online\] 6 Sep. Available at:
    > [<u>https://www.reuters.com/article/us-michaeljackson-life-idUSTRE7852M420110906</u>](https://www.reuters.com/article/us-michaeljackson-life-idUSTRE7852M420110906).

‌

-   Okwerekwu, I. (2019). *Tupac: The Greatest Inspirational Hip Hop
    > Artist*. \[online\] Medium. Available at:
    > [<u>https://medium.com/music-for-inspiration/tupac-the-greatest-inspirational-hip-hop-artist-7118f02747ed</u>](https://medium.com/music-for-inspiration/tupac-the-greatest-inspirational-hip-hop-artist-7118f02747ed)

<!-- -->

-   Wikipedia. (2024). *Steve Biko*. \[online\] Available at:
    > [<u>https://en.wikipedia.org/wiki/Steve_Biko#CITEREFWoods1978</u>](https://en.wikipedia.org/wiki/Steve_Biko)
    > \[Accessed 12 Mar. 2024\].

‌

‌

-   ‌Biographical Memoirs of Fellows of the Royal Society. (2016).
    > *Albert Einstein, 1879-1955 \| Biographical Memoirs of Fellows of
    > the Royal Society*. \[online\] Available at:
    > [<u>https://doi.org/10.1098%2Frsbm.1955.0005</u>](https://doi.org/10.1098%2Frsbm.1955.0005)

<!-- -->

-   web.archive.org. (2016). *How it all began*. \[online\] Available
    > at:
    > [<u>https://web.archive.org/web/20160819021657/http://www.mercedes-benz.co.ke/content/kenya/mpc/mpc_kenya_website/en/home_mpc/passengercars/home/world/mythos/how_it_began.html</u>](https://web.archive.org/web/20160819021657/http://www.mercedes-benz.co.ke/content/kenya/mpc/mpc_kenya_website/en/home_mpc/passengercars/home/world/mythos/how_it_began.html)
    > \[Accessed 12 Mar. 2024\].

<!-- -->

-   Wikipedia. (2024). *British subject*. \[online\] Available at:
    > [<u>https://en.wikipedia.org/wiki/British_subject</u>](https://en.wikipedia.org/wiki/British_subject)
    > \[Accessed 12 Mar. 2024\].

<!-- -->

-   iasl.uni-muenchen.de. (n.d.). *IASLonline NetArt: History of
    > Computer Art VII.1 Computer and Video Games*. \[online\] Available
    > at:
    > [<u>http://iasl.uni-muenchen.de/links/GCA-VII.1e.html#top17</u>](http://iasl.uni-muenchen.de/links/GCA-VII.1e.html)
    > \[Accessed 12 Mar. 2024\].

<!-- -->

-   Staff, W. (2009). *Dec. 18, 1878: Let There Be Light — Electric
    > Light*. \[online\] WIRED. Available at:
    > [<u>https://www.wired.com/2009/12/1218joseph-swan-electric-bulb/</u>](https://www.wired.com/2009/12/1218joseph-swan-electric-bulb/).
