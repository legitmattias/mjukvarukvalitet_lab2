# Test Report
Project: Mjukvarukvalitet L2
Date: 2024-10-02
Name: Mattias Ubbesen <mu222cu@student.lnu.se>

## Test Results

### `ChangelogProcessor`
- ✓ should extract unreleased changes (6 ms)
- ✓ should extract added features (1 ms)
- ✓ should extract changed features (1 ms)
- ✓ should extract deprecated features (1 ms)
- ✓ should extract removed features
- ✓ should extract bug fixes
- ✓ should extract security updates (1 ms)
- ✓ should get updates between two close versions 2.2.1 and 2.2.0 (1 ms)
- ✓ should throw error if no updates found between two versions (8 ms)

### `RepoReadmeProcessor`
- ✓ should extract installation instructions (4 ms)
- ✓ should extract usage examples
- ✓ should extract API documentation (1 ms)
- ✓ should extract configuration information
- ✓ should extract dependencies list
- ✓ should extract contribution guidelines
- ✓ should extract license information (1 ms)
- ✓ should extract the project title and description

### `NpmReadmeProcessor`
- ✓ should extract CLI usage information (4 ms)
- ✓ should extract versioning details (1 ms)
- ✓ should extract scripts information

### `MarkdownParser`
- ✓ should read and parse hash-style markdown content (5 ms)
- ✓ should return the correct title from hash-style markdown (1 ms)
- ✓ should read and parse underline-style markdown content
- ✓ should count headings by level in underline-style markdown (1 ms)
- ✓ should read and parse markdown content (combination of notations)
- ✓ should return the correct title from combination markdown
- ✓ should count headings by level from combination markdown (1 ms)
- ✓ should return the count of headings for a specific level from combination markdown
- ✓ should return sections with matching heading keyword from combination markdown (1 ms)
- ✓ should throw an error if no sections match the keyword from combination markdown (8 ms)

### `MarkdownParser - Dictionary Methods`
- ✓ should return the dictionary object
- ✓ should return keywords for a specific section type (1 ms)
- ✓ should add a keyword to a section type

## Coverage Summary

| File                    | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s                           |
|-------------------------|---------|----------|---------|---------|---------------------------------------------|
| All files               | 86.75   | 68.57    | 100     | 87.16   |                                             |
| `ChangelogProcessor.ts`  | 96.15   | 80       | 100     | 96.15   | 132                                         |
| `HeadingDictionary.ts`   | 75      | 42.85    | 100     | 75      | 62-65, 98                                   |
| `MarkdownParser.ts`      | 83.72   | 69.04    | 100     | 84.52   | 79, 97, 103-108, 191, 214, 265, 279, 310, 355, 379 |
| `NpmReadmeProcessor.ts`  | 100     | 80       | 100     | 100     | 43                                          |
| `RepoReadmeProcessor.ts` | 93.75   | 66.66    | 100     | 93.33   | 125                                         |

## Summary

- **Test Suites:** 4 passed, 4 total
- **Tests:** 33 passed, 33 total
- **Snapshots:** 0 total
- **Time:** 1.569 s
- **Ran all test suites**

