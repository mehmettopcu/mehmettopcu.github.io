# Welcome to My GitHub Pages

This page showcases all of my public repositories on GitHub. You can explore the various projects I've worked on and contribute if you'd like!

## My GitHub Repositories

<ul id="repo-list">
  <!-- Repositories will be loaded here -->
</ul>

<script>
  // Replace with your GitHub username
  const username = 'mehmettopcu';

  fetch(`https://api.github.com/users/${username}/repos`)
    .then(response => response.json())
    .then(repos => {
      const repoList = document.getElementById('repo-list');
      repos.forEach(repo => {
        const repoItem = document.createElement('li');
        repoItem.innerHTML = `<a href="https://github.com/${repo.owner.login}/${repo.name}">${repo.name}</a> - ${repo.description || 'No description available'}`;
        repoList.appendChild(repoItem);
      });
    })
    .catch(error => console.error('Error fetching repositories:', error));
</script>

## About Me

I am an experienced OpenStack expert, DevOps engineer, and system administrator with a strong background in automation and cloud-native technologies. I specialize in deploying and managing scalable systems, orchestrating Kubernetes clusters, and integrating DevOps practices into the development lifecycle.

Feel free to check out my repositories, and don't hesitate to open an issue or pull request if you want to contribute!

## Contact

- GitHub: [@mehmettopcu](https://github.com/mehmettopcu)

### Support or Questions

If you have any questions about my repositories or would like to collaborate, feel free to reach out via [email](mailto:your-email@example.com) or open an issue in one of the repositories.
