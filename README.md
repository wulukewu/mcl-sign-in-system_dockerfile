# MCL Automatic Sign-in System

![GitHub last commit](https://img.shields.io/github/last-commit/wulukewu/mcl-sign-in-system?style=for-the-badge)
![GitHub issues](https://img.shields.io/github/issues/wulukewu/mcl-sign-in-system?style=for-the-badge)
![Docker Pulls](https://img.shields.io/docker/pulls/wulukewu/mcl-sign-in-system?style=for-the-badge)
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/wulukewu/mcl-sign-in-system/latest?label=latest%20image%20size&style=for-the-badge)

An auto sign-in/sign-out system for NCU HumanSys. 

## Hub

**GitHub**: [wulukewu/mcl-sign-in-system](https://github.com/wulukewu/mcl-sign-in-system)

**Docker Hub**: [wulukewu/mcl-sign-in-system](https://hub.docker.com/r/wulukewu/mcl-sign-in-system)

To automatically run this Docker on GitHub Actions, see this repository: [wulukewu/mcl-sign-in-system-runner](https://github.com/wulukewu/mcl-sign-in-system-runner)

## Parameters

- **`--inorout`**: Specify `"signin"` or `"signout"` for the desired action.
- **`--username`**: Your Student ID used for login.
- **`--password`**: Password for your portal login.
- **`--otpauth`** [optional]: OTP URL to generate a one-time password (OTP) for two-factor authentication.

## Usage

To run the script, use the following command:

```sh
python main.py --inorout <signin|signout> --username <your_username> --password <your_password> --otpauth <[optional] otpauth_url>
```

## Docker

To build and run the Docker container, use the following commands:

```sh
docker build -t mcl-sign-in-system .
docker run mcl-sign-in-system --inorout <signin|signout> --username <your_username> --password <your_password> --otpauth <[optional] otpauth_url>
```

## References

- [VS Code + Python + Selenium Automation Testing Part 1](https://medium.com/begonia-design/vs-code-python-selenium-%E8%87%AA%E5%8B%95%E5%8C%96%E6%B8%AC%E8%A9%A6-part-1-30d6c0ea92af)

- [Day 15: Dynamic Web Page Scraping 2 - Selenium Data Location Functions](https://ithelp.ithome.com.tw/articles/10300961)

- [【 Python 】利用 .env 與環境變數隱藏敏感資訊](https://learningsky.io/python-use-environmental-variables-to-hide-sensitive-information/)

- [Pull a certain branch from the remote server](https://stackoverflow.com/questions/1709177/pull-a-certain-branch-from-the-remote-server)

- [recaptcha_v2_solver](https://github.com/ohyicong/recaptcha_v2_solver)
