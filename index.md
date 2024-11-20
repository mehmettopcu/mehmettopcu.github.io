# Welcome to My GitHub Pages

This page showcases all of my public repositories on GitHub. You can explore the various projects I've worked on and contribute if you'd like!

## My GitHub Repositories

Here are some of my most notable repositories:

<ul>
  {% for repo in site.github.repositories %}
    <li>
      <a href="https://github.com/{{ repo.owner.login }}/{{ repo.name }}">
        {{ repo.name }}
      </a>
      - {{ repo.description | default: "No description available" }}
    </li>
  {% endfor %}
</ul>

## About Me

I am a software developer with a passion for open-source projects. My work includes everything from web development to data science and automation tools.

Feel free to check out my repositories, and don't hesitate to open an issue or pull request if you want to contribute!

## Contact

- GitHub: [@mehmettopcu](https://github.com/mehmettopcu)
- Email: [your-email@example.com](mailto:your-email@example.com)

### Support or Questions

If you have any questions about my repositories or would like to collaborate, feel free to reach out via [email](mailto:your-email@example.com) or open an issue in one of the repositories.
