
# 💫 About Me:
Hi 👋, I'm Akhil, A passionate DevOps Engineer from India<br>🌱 I’m currently learning **DevOps Tools

## 🏆 GitHub Trophies

![](https://github-profile-trophy.vercel.app/?username=akhil2099&theme=juicyfresh&no-frame=true&no-bg=false&margin-w=4)
![](https://quotes-github-readme.vercel.app/api?type=vetical&theme=radical)






## 🌐 Socials:
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/shooto_gram) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/akhil-v-953b04275) [![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=Twitter&logoColor=white)](https://twitter.com/@zeuz1234567890) [![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?logo=YouTube&logoColor=white)](https://youtube.com/@@shootogram7270) 

# 💻 Tech Stack:
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white) ![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=azure-devops&logoColor=white) ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white) ![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Ansible](https://img.shields.io/badge/ansible-%231A1918.svg?style=for-the-badge&logo=ansible&logoColor=white) ![LINUX](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Ansible](https://img.shields.io/badge/ansible-%231A1918.svg?style=for-the-badge&logo=ansible&logoColor=white) ![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white) ![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=akhil2099&theme=radical&hide_border=false&include_all_commits=true&count_private=false)
![](https://github-readme-streak-stats.herokuapp.com/?user=akhil2099&theme=radical&hide_border=false)<br/>

![](https://github-readme-stats.vercel.app/api/top-langs/?username=akhil2099&theme=radical&hide_border=false&include_all_commits=true&count_private=false&layout=compact)


---
[![](https://visitcount.itsvg.in/api?id=akhil2099&icon=2&color=9)](https://visitcount.itsvg.in)

import matplotlib.pyplot as plt
import numpy as np

# Sample data for contributions (replace this with your actual data)
contributions = np.random.randint(0, 6, (7, 52))

# Define the labels for the weekdays and months
weekdays = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
months = [
    'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
    'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'
]

def plot_contribution_graph(contributions):
    fig, ax = plt.subplots(figsize=(10, 6))
    im = ax.imshow(contributions, cmap='Blues')

    # Show color bar
    cbar = ax.figure.colorbar(im, ax=ax)
    cbar.ax.set_ylabel("Contributions", rotation=-90, va="bottom")

    # Set the ticks and labels for x and y-axes
    ax.set_xticks(np.arange(len(weekdays)))
    ax.set_yticks(np.arange(len(months)))
    ax.set_xticklabels(weekdays)
    ax.set_yticklabels(months)

    # Rotate the tick labels and set their alignment
    plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")

    # Loop over data dimensions and create text annotations.
    for i in range(len(months)):
        for j in range(len(weekdays)):
            text = ax.text(j, i, contributions[i, j],
                           ha="center", va="center", color="w")

    ax.set_title("GitHub Contribution Graph")
    fig.tight_layout()
    plt.show()

# Call the function to plot the contribution graph
plot_contribution_graph(contributions)
