## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Whitey2071/DRL_for_Assistive_Vision/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Whitey2071/DRL_for_Assistive_Vision/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


### Supplementary Material
This page displays the saliency and feature map videos referenced in the paper "Vision Processing for Assistive Vision: A Deep Reinforcement Learning Approach". The two videos shown below were rendered using single frames that were individually passed to the trained Deep Neural Network (DNN) and then collated to produce these videos. 

## Saliency Video:
Our saliency video was produced using the saliency algorithm by Greydanus et al. (https://github.com/greydanus/visualize_atari). On each single frame a saliency map is rendered that is then overlayed on the original grayscale image. Highlighted regions in the frames displayed in the video indicate areas of importance for the agent to make an action selection since saliency is based on the predicted policy output. A key outcome from this video is that the agent can dynamically make decisions based upon a rapidly changing context and the task it is presented with. Thus, images that are passed to the DNN are filtered and produce a policy output based on the context of the input image. Further, this video explains some of the agent's behaviour and its tendency to focus on certain features of particular importance for it to effectively navigate. In particular, the agent can be seen focusing areas with high levels of depth and edges at the wall-sky interface. However, regions of high depth are prioritised if the agent is planning on traversing toward that area of the maze as is made evident by the video below. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/ylgkQkxRAtY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Each individual image produces a set of filter responses from the trained convolutional 

Feature Map Video:

<iframe width="560" height="315" src="https://www.youtube.com/embed/9OCJqV4tCAg" frameborder="0" allow="accelerometer; autoplay; encrypted-media" allowfullscreen></iframe>
