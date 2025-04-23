# Automated-SonarQube-Integration at Enterprise level 


## 📌 Overview

This project showcases how I led the automation of SonarQube integration across hundreds of Java repositories at American Express. The goal was to ensure consistent code quality, improve test coverage tracking, and reduce manual onboarding friction for developers.

## 🔍 Problem Statement

- Developers lacked consistent visibility into code quality and test coverage.
- Manual SonarQube onboarding was slow, error-prone, and not scalable.
- Compliance and security teams required centralized metrics from all Java services.

## 🎯 Objective

- Build an internal automation tool to integrate SonarQube into existing Java repositories.
- Automate SonarQube setup across all Java repos.
- Generate PRs to onboard repositories with a consistent coverage workflow.
- Notify repo owners and track adoption.

## 🛠️ My Role

The first milestone was to develop a lightweight automation tool that programmatically injected SonarQube configuration into each targeted repository and created pull requests. This served as the foundation for later phases of automation and tracking.

As the **Solution Architect and Team Lead**, I:
- Designed the automation flow and architecture
- Wrote scripts in Go and Shell for GitHub automation
- Integrated GitHub CLI for PR creation and validation
- Led platform-wide coordination for secure token and permission setup
- Drove collaboration across product, DevOps, and compliance teams
- Mentored junior engineers and reviewed implementation contributions

## 🧰 Tech Stack

- **Languages**: Go, Bash
- **DevOps Tools**: GitHub CLI, GitHub Actions
- **CI/CD**: SonarQube, Jenkins
- **Scripting & Automation**: Custom CLI wrappers, GitHub workflows
- **Monitoring**: Scripted checks for PR status, repo coverage compliance

## 🔄 How the Automation Works (Quick Summary)

- ✅ Detects programming language and build tool for each repo (e.g., Java + Maven)
- 🛠️ Checks if the repo is already onboarded to SonarQube
- 📄 Injects `sonar-project.properties` and workflow YAML files
- 🤖 Uses GitHub CLI to raise a pull request
- ⚙️ Triggers GitHub Actions to validate the integration
- 📨 Notifies repo owners and tracks status for compliance

📘 **For the full architecture and implementation**, see [DETAILS.md](./DETAILS.md)
