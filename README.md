# ISMRM Iberian Chapter

To run locally the website:

1. Follow the guide from the Jekill website to install it depending on your operating system:
    - [macOS](https://jekyllrb.com/docs/installation/macos/)
    - [Windows](https://jekyllrb.com/docs/installation/windows/)
    - [Ubuntu](https://jekyllrb.com/docs/installation/ubuntu/)

2. Open CLI and change the current working directory to the location where you want the cloned directory.
3. Clone the repository by using:

   ```bash
   git clone https://github.com/ismrm-iberian/ismrm-iberian.github.io.git
   ```

4. Change the current directory to the repository cloned:

   ```bash
   cd ismrm-iberian.github.io
   ```

5. Delete the Gemfile.lock to be able to get new versions
6. To fix a known error of bundler, run in CLI:

     ```bash
    bundle config set --local force_ruby_platform true
    ```

7. To create a new Gemfile.lock and install the requirements, run in CLI:

   ```bash
   bundle install
   ```

8. Start the local server with live reload enable, to automatically refresh the page with each change you make to the source files:

   ```bash
   bundle exec jekyll serve --livereload
   ```
