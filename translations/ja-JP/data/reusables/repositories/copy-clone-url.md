{% if currentVersion != "free-pro-team@latest" and currentVersion ver_lt "enterprise-server@2.22" %}
1. リポジトリ名の下で**Clone or download（クローンもしくはダウンロード）**をクリックしてください。 ![Clone or downloadボタン](/assets/images/help/repository/clone-repo-clone-url-button.png)
2. To clone the repository using HTTPS, under "Clone with HTTPS", click
{% octicon "clippy" aria-label="The clipboard icon" %}.
To clone the repository using an SSH key
{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.18" %}, including a certificate issued by your organization's SSH certificate authority,{% endif %} click **Use SSH**, then click {% octicon "clippy" aria-label="The clipboard icon" %}.
![クローンURLボタン](/assets/images/help/repository/https-url-clone.png)
{% else %}
1. Above the list of files, click {% octicon "download" aria-label="The download icon" %} **Code**. !["Code" button](/assets/images/help/repository/code-button.png)
1. To clone the repository using HTTPS, under "Clone with HTTPS", click
{% octicon "clippy" aria-label="The clipboard icon" %}. To clone the repository using an SSH key{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.18" %}, including a certificate issued by your organization's SSH certificate authority,{% endif %} click **Use SSH**, then click {% octicon "clippy" aria-label="The clipboard icon" %}.{% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.22" %} To clone a repository using {{ site.data.variables.product.prodname_cli }}, click **Use {{ site.data.variables.product.prodname_cli }}**, then click {% octicon "clippy" aria-label="The clipboard icon" %}.{% endif %}
  ![The clipboard icon for copying the URL to clone a repository](/assets/images/help/repository/https-url-clone.png)
  {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.19" %}
  ![The clipboard icon for copying the URL to clone a repository with GitHub CLI](/assets/images/help/repository/https-url-clone-cli.png){% endif %}
{% endif %}