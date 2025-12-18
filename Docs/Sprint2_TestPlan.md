# Sprint 2 Test Plan - Legacy of Lost

## Scope
Sprint 2 introduces combat mechanics and includes regression testing of Sprint 1 features.

## New Modules Tested

### 3. Battle Powerful Enemies to Develop Strategies (TC003)
- **Description**: Verify combat system with enemy AI interactions
- **Expected Result**: Player can engage enemies, damage calculation works correctly
- **Priority**: High

## Regression Testing
Sprint 2 includes regression tests to ensure previous functionality remains intact:
- TC001: Control Unique Main Character
- TC002: Unlock New Skills After Defeating Chapter Boss

## CI/CD Integration
- **Pipeline**: GitHub Actions workflow `LegacyOfLost-CI`
- **Trigger**: On push to master branch
- **Test Tool**: GameDriver automated testing framework
- **Test Cases**: TC001, TC002, TC003 (including regression)

## Sprint 2 Results
All tests executed successfully via CI/CD pipeline:
- ✅ TC001: Control Unique Main Character - PASS (Regression)
- ✅ TC002: Unlock New Skills After Defeating Chapter Boss - PASS (Regression)
- ✅ TC003: Battle Powerful Enemies to Develop Strategies - PASS (New Feature)

## Regression Testing Benefits
By running all previous tests alongside new tests, we ensure:
- No breaking changes to existing features
- New features integrate smoothly with existing code
- Continuous quality assurance across sprints

Test results are automatically generated and stored as artifacts in GitHub Actions.
