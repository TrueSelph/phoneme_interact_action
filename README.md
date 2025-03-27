# Phoneme Interact Action

![GitHub release (latest by date)](https://img.shields.io/github/v/release/TrueSelph/phoneme_interact_action)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/TrueSelph/phoneme_interact_action/test-action.yaml)
![GitHub issues](https://img.shields.io/github/issues/TrueSelph/phoneme_interact_action)
![GitHub pull requests](https://img.shields.io/github/issues-pr/TrueSelph/phoneme_interact_action)
![GitHub](https://img.shields.io/github/license/TrueSelph/phoneme_interact_action)

JIVAS action for managing phoneme-based prompting to customize the pronunciation of words for text-to-speech models.

## Package Information

- **Name:** `jivas/phoneme_interact_action`
- **Author:** [V75 Inc.](https://v75inc.com/)
- **Architype:** `PhonemeInteractAction`

## Meta Information

- **Title:** Phoneme Interact Action
- **Group:** core
- **Type:** interact_action

## Configuration

- **Singleton:** false
- **Order:**
  - **Weight:** 0
  - **After:** `persona_interact_action`

## Dependencies

- **Jivas:** `^2.0.0`
- **Actions:**
  - `jivas/persona_interact_action`: `^0.0.1`
- **Pip:**
  - `types-PyYAML`
  - `types-requests`

This package, developed by V75 Inc., manages phoneme-based prompting, enabling customization of word pronunciations for text-to-speech models used by an agent. As a core interact action, it enhances speech output quality and accuracy. It requires the Jivas library version 2.0.0 and depends on the `persona_interact_action` for extended functionality.

---

## How to Use

Below is detailed guidance on how to configure and use the Phoneme Interact Action.

### Overview

The Phoneme Interact Action provides an abstraction layer for managing phoneme-based prompting. It supports multiple configurations for various use cases, including:

- **Custom phoneme mappings** for specific words.
- **Integration** with text-to-speech engines.
- **Dynamic phoneme editing** via the app interface.

---

### Configuration Structure

The configuration consists of the following components:

### `phonemes`

Defines the phoneme mappings for words, where the key is the word, and the value is its phonetic representation.

```python
phonemes = {
    "example": "ɪɡˈzæmpəl",  # Example in IPA
    "data": "ˈdeɪtə",        # Example in IPA
}
```

---

### Example Configurations

### Basic Phoneme Mapping

```python
phonemes = {
    "hello": "həˈloʊ",
    "world": "wɜːrld",
}
```

### Best Practices
- Validate phoneme mappings for compatibility with your TTS engine.
- Test configurations in a staging environment before production use.

---

## 🔰 Contributing

- **🐛 [Report Issues](https://github.com/TrueSelph/phoneme_interact_action/issues)**: Submit bugs found or log feature requests for the `phoneme_interact_action` project.
- **💡 [Submit Pull Requests](https://github.com/TrueSelph/phoneme_interact_action/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your GitHub account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/TrueSelph/phoneme_interact_action
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to GitHub**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!
</details>

<details open>
<summary>Contributor Graph</summary>
<br>
<p align="left">
    <a href="https://github.com/TrueSelph/phoneme_interact_action/graphs/contributors">
        <img src="https://contrib.rocks/image?repo=TrueSelph/phoneme_interact_action" />
   </a>
</p>
</details>

## 🎗 License

This project is protected under the Apache License 2.0. See [LICENSE](./LICENSE) for more information.