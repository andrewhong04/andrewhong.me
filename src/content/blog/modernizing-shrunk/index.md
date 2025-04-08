---
title: "Modernizing the URL Shortener for Rutgers Office of Information Technology used by thousands of faculty members"
description: "From old to new."
date: "Apr 7 2025"
---

What? A URL Shortener? Sounds like a simple project. If you incorporate the state it was in before I started the revamp, it was kindof messy. The build process incorporated a symbolic link to be used to link the frontend to the backend, three terminal processes to be running (NodeJS, Flask, and MongoDB), and `requirements.txt` was used to lock in dependencies instead of a dedicated package manager. These were some of the things I addressed that managed to make the developer experience a lot smoother.

![Shrunk using Docker](/shrunk-docker.png)

## Main Concerns

- UI is outdated; sharp corner boxes are out, rounded boxes are in
- Design philosophy is all out of place, CSS is used everywhere to modify components to add personality to them but it looks like it's been overdone to the point where the whole design became inconsistent
- Two icon libraries are used [react-icons](https://react-icons.github.io/react-icons/) and [@ant-design/icons](https://github.com/ant-design/ant-design-icons)
- Full-stack project is not dockerized, hassle to even start working on the project
- Proper package manager isn't used, backend dependency conflicts happen when trying to install everything to the virtual environment
- [iCloud Private Relay](https://support.apple.com/en-us/102602) is not supported
- Admin control panel is not optimized, it loads all the users before displaying them
- Everything from API tokens, settings, and etc were stored in `config.py` instead of environment variables
- Shrunk served some HTML files from Flask instead of React such as the login page, 404, etc

## New Design

There's really not much to say about the changes, they're just design changes influenced by me accumulating ideas for a couple months.

Once everything is complete, the entire before and after comparison will be implemented.

### Splash Screen

![Old Shrunk Splash Page](/old-shrunk.png)

![New Shrunk Splash Page](/new-shrunk.png)
