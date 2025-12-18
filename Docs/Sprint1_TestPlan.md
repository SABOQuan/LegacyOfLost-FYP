# Sprint 1 Test Plan - Legacy of Lost

## Scope
Sprint 1 focuses on core gameplay mechanics and basic player interactions.

## Modules Tested

### 1. Control Unique Main Character (TC001)
- **Description**: Verify player can control the main character using WASD keys
- **Expected Result**: Character moves in all directions, responds to jump input
- **Priority**: High

### 2. Unlock New Skills After Defeating Chapter Boss (TC002)
- **Description**: Verify skill unlock system triggers after boss defeat
- **Expected Result**: New skills are added to player inventory
- **Priority**: High

## CI/CD Integration
- **Pipeline**: GitHub Actions workflow `LegacyOfLost-CI`
- **Trigger**: On push to master branch
- **Test Tool**: GameDriver automated testing framework
- **Test Cases**: TC001, TC002

## Sprint 1 Results
All tests executed successfully via CI/CD pipeline:
- ✅ TC001: Control Unique Main Character - PASS
- ✅ TC002: Unlock New Skills After Defeating Chapter Boss - PASS

Test results are automatically generated and stored as artifacts in GitHub Actions.
