<header>

<!--
  <<< Author notes: Course header >>>
  Include a 1280×640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Add your open source license, GitHub uses MIT license.
-->

# Introduction to ROS2

_Get started developping robotics applications using ros2._

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: Install ROS2 Humble


**1.1: Download and Install ROS 2 Humble**
**1.2:  Configuration and setup of the developpement environnement**
**1.3: Extra useful app and tools**

**1.1: Download and Install ROS 2 Humble**: 
Download and install Ubuntu 22.04 image:
https://cdimage.ubuntu.com/jammy/daily-live/current/

Choose desktop image file based on your machine architecture: amd vs arm
<p> Set locale: <p>
locale  # check for UTF-8
sudo apt update && sudo apt install locales
sudo locale-gen en_US en_US.UTF-8
sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
export LANG=en_US.UTF-8
locale  # verify settings![image](https://github.com/user-attachments/assets/721d8ee6-3d62-4dc7-9737-78d8485d7ee9)

<p> Setup sources:</p>
sudo apt install software-properties-common
sudo add-apt-repository universe
sudo apt update && sudo apt install curl -y
sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null

<p> Install ROS 2 packages </p>
sudo apt update
sudo apt upgrade
sudo apt install ros-humble-desktop
sudo apt install ros-dev-tools	
![image](https://github.com/user-attachments/assets/911db42f-457e-4b47-90d9-236270a95ae0)



**What is a repository?**: A _[repository](https://docs.github.com/get-started/quickstart/github-glossary#repository)_ is a project containing files and folders. A repository tracks versions of files and folders. For more information, see "[About repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories)" from GitHub Docs.

**What is a branch?**: A _[branch](https://docs.github.com/en/get-started/quickstart/github-glossary#branch)_ is a parallel version of your repository. By default, your repository has one branch named `main` and it is considered to be the definitive branch. Creating additional branches allows you to copy the `main` branch of your repository and safely make any changes without disrupting the main project. Many people use branches to work on specific features without affecting any other parts of the project.

Branches allow you to separate your work from the `main` branch. In other words, everyone's work is safe while you contribute. For more information, see "[About branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches)".

**What is a profile README?**: A _[profile README](https://docs.github.com/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)_ is essentially an "About me" section on your GitHub profile where you can share information about yourself with the community on GitHub.com. GitHub shows your profile README at the top of your profile page. For more information, see "[Managing your profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)".

![profile-readme-example](/images/profile-readme-example.png)

### :keyboard: Activity: Your first branch

1. Open a new browser tab and navigate to your newly made repository. Then, work on the steps in your second tab while you read the instructions in this tab.
2. Navigate to the **< > Code** tab in the header menu of your repository.

   ![code-tab](/images/code-tab.png)

3. Click on the **main** branch drop-down.

   ![main-branch-dropdown](/images/main-branch-dropdown.png)

4. In the field, name your branch `my-first-branch`. In this case, the name must be `my-first-branch` to trigger the course workflow.
5. Click **Create branch: my-first-branch** to create your branch.

   ![create-branch-button](/images/create-branch-button.png)

   The branch will automatically switch to the one you have just created.
   The **main** branch drop-down bar will reflect your new branch and display the new branch name.

6. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/introduction-to-github) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2024 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
