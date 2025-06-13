# Changelog

All notable changes to the dataset cleaning process are documented in this file.

## [Unreleased]

### Changed
- **Column names**: Trimmed whitespace, converted to lowercase, and replaced spaces with underscores.
- **Object names**: Lowercased, underscored, and corrected typos using canonical mapping (`laptp` → `laptop`, `whitebored` → `whiteboard`, `mug_` → `coffee_mug`).
- **Object categories**: Trimmed whitespace, lowercased, and underscored to standardize category labels.
- **Missing confidence**: Filled null `confidence` values with the median confidence score.

### Added
- **Schema validation**: Checked presence of all required fields from `schema_map_6.12.25.csv`.
- **Bounding-box checks**: Verified that `x_max > x_min` and `y_max > y_min` for all boxes.
- **Duplicate detection**: Ensured there are no duplicate rows based on `frame_id` and bounding-box coordinates.

## [0.1.0] - 2025-06-12
### Added
- Initial data cleanup log following the Keep a Changelog format.

