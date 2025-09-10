# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.1] - 2025-09-10

### Changed (0.1.1)

- Simplified release automation: removed duplicate dispatch/bridge workflows to avoid multiple release runs.
- Fixed PyInstaller build to produce single-file Windows executable (`MyPyTemplate.exe`).
- Corrected tagging flow to trigger release only once per version tag.

### Fixed (0.1.1)

- Missing `fi` in workflow causing syntax error in tag verification step.
- Incorrect `--add-data` syntax for PyInstaller on Windows.
- Badge generation step indentation and version extraction issues.

### Internal (0.1.1)

- Adopted PAT usage pattern (RELEASE_PAT) reserved for future enabling; current workflow expects existing PAT for tag push.

## [0.1.0] - 2025-09-10

### Added (0.1.0)

- Initial project scaffolding with modern Python packaging (`pyproject.toml`)
- Console command `MyPyTemplate`
- **Windows executable (.exe) generation with PyInstaller**
- Complete CI/CD pipeline with GitHub Actions (lint, test, build, deploy)
- Multi-platform release builds (Python packages + Windows executable)
- Code quality tools: Ruff, Black, Mypy, Pytest
- Dynamic versioning from `version_info.txt`
- Automated version bumping from changelog
- Development environment with editable install and dev dependencies
- Basic module structure with `core.main`, `core.version`, `core.utils`
- Test suite with pytest configuration
- Documentation structure with README and changelog
