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


**1.1: Download and Install ROS 2 Humble** <br>
**1.2: Configuration and setup of the developpement environnement**<br>
**1.3: Extra useful app and tools**<br>

**1.1: Download and Install ROS 2 Humble**: 
Download and install Ubuntu 22.04 image:<br>
https://cdimage.ubuntu.com/jammy/daily-live/current/

Choose desktop image file based on your machine architecture: amd vs arm <br>

<p> <em> Set locale: </em> <p> 
locale  # check for UTF-8 <br>
sudo apt update && sudo apt install locales <br>
sudo locale-gen en_US en_US.UTF-8<br>
sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8 <br>
export LANG=en_US.UTF-8 <br>
locale  # verify settings! <br>

<p> Setup sources:</p>
sudo apt install software-properties-common <br>
sudo add-apt-repository universe <br>
sudo apt update && sudo apt install curl -y <br>
sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null<br>
<p> Install ROS 2 packages </p>
sudo apt update <br>
sudo apt upgrade <br>
sudo apt install ros-humble-desktop <br>
sudo apt install ros-dev-tools	<br>

**1.2: Configuration and setup of the developpement environnement**<br>

**1.3: Extra useful app and tools**<br>


<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/introduction-to-github) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2024 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
