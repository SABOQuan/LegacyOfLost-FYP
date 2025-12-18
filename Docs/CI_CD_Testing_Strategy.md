# CI/CD and Automated Testing Strategy

## Overview
This document outlines the CI/CD pipeline and automated testing approach for Legacy of Lost Unity FYP project.

## CI/CD Pipeline Architecture

### GitHub Actions Workflow
- **Name**: LegacyOfLost-CI
- **Location**: `.github/workflows/unity-gamedriver-tests.yml`
- **Trigger**: Push to master branch or pull request
- **Platform**: Windows Latest

### Pipeline Steps
1. **Checkout Repository**: Clone the latest code
2. **Setup Unity Environment**: Configure Unity test environment
3. **Run GameDriver Tests**: Execute automated regression tests
4. **Upload Artifacts**: Store test results for review

## Automated Testing Framework

### GameDriver Integration
GameDriver is used for automated Unity game testing:
- Simulates player input and interactions
- Validates game mechanics and behavior
- Generates detailed test reports

### Test Cases

#### Sprint 1
- **TC001**: Control Unique Main Character
- **TC002**: Unlock New Skills After Defeating Chapter Boss

#### Sprint 2 (includes regression)
- **TC001**: Control Unique Main Character (Regression)
- **TC002**: Unlock New Skills After Defeating Chapter Boss (Regression)
- **TC003**: Battle Powerful Enemies to Develop Strategies (New)

## Benefits of CI/CD Approach

1. **Automated Regression Testing**: Every code push runs full test suite
2. **Early Bug Detection**: Issues caught before reaching production
3. **Consistent Testing**: Same tests run in same environment every time
4. **Documentation**: Test artifacts provide audit trail
5. **Time Savings**: Automated testing faster than manual testing

## Test Artifacts
Each workflow run generates:
- `GameDriverTestResults.txt`: Detailed test execution results
- Console logs: Step-by-step execution output
- Timestamps: When tests were executed

## Sprint Workflow
1. Developer pushes code changes to master
2. GitHub Actions automatically triggers workflow
3. Workflow runs all test cases (including regression)
4. Test results uploaded as artifacts
5. Team reviews results and test reports
