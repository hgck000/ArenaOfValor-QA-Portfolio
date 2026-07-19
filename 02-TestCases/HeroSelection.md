# Hero Selection Test Suite

## Module Information

| Item             | Value              |
| ---------------- | ------------------ |
| Module           | Hero Selection     |
| Test Type        | Functional Testing |
| Tester           | Quang Minh         |
| Platform         | Android            |
| Total Test Cases | 10                 |
| Passed           | 10                 |
| Failed           | 0                  |
| Blocked          | 0                  |
| Test Result      | ✅ PASS            |

---

## Covered Requirements

| Requirement ID | Description                                       |
| -------------- | ------------------------------------------------- |
| HERO-REQ-001   | Player can select an available hero               |
| HERO-REQ-002   | Player can change selected hero before locking    |
| HERO-REQ-003   | Player can lock selected hero                     |
| HERO-REQ-004   | Hero selection countdown functions correctly      |
| HERO-REQ-005   | Hero customization can be modified before locking |

---

## AOV-TC-HERO-001

| Field         | Value                             |
| ------------- | --------------------------------- |
| Title         | Select an available hero          |
| Priority      | High                              |
| Preconditions | Hero Selection phase has started. |
| Test Data     | Any available hero                |

### Test Steps

1. Enter Hero Selection.
2. Select an available hero.

### Expected Result

The selected hero is displayed correctly.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-002

| Field         | Value                      |
| ------------- | -------------------------- |
| Title         | Change hero before locking |
| Priority      | High                       |
| Preconditions | Hero has been selected.    |

### Test Steps

1. Select Hero A.
2. Select Hero B before locking.

### Expected Result

Hero selection changes successfully.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-003

| Field         | Value                   |
| ------------- | ----------------------- |
| Title         | Lock selected hero      |
| Priority      | High                    |
| Preconditions | Hero has been selected. |

### Test Steps

1. Select any hero.
2. Press **Lock**.

### Expected Result

Selected hero is locked successfully.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-004

| Field         | Value                                |
| ------------- | ------------------------------------ |
| Title         | Attempt to change hero after locking |
| Priority      | Medium                               |
| Preconditions | Hero has been locked.                |

### Test Steps

1. Lock Hero A.
2. Attempt to select Hero B.

### Expected Result

Hero cannot be changed after locking.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-005

| Field         | Value                              |
| ------------- | ---------------------------------- |
| Title         | Change skin before locking         |
| Priority      | Medium                             |
| Preconditions | Hero selected with multiple skins. |

### Test Steps

1. Select a hero.
2. Change to another skin.
3. Lock hero.

### Expected Result

Selected skin is applied successfully.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-006

| Field    | Value                        |
| -------- | ---------------------------- |
| Title    | Change Arcana before locking |
| Priority | Medium                       |

### Test Steps

1. Select a hero.
2. Change Arcana page.
3. Lock hero.

### Expected Result

Selected Arcana page is applied.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-007

| Field    | Value                        |
| -------- | ---------------------------- |
| Title    | Change Talent before locking |
| Priority | Medium                       |

### Test Steps

1. Select a hero.
2. Change Talent.
3. Lock hero.

### Expected Result

Selected Talent is applied.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-008

| Field    | Value                           |
| -------- | ------------------------------- |
| Title    | Reconnect during Hero Selection |
| Priority | High                            |

### Test Steps

1. Enter Hero Selection.
2. Disconnect the network.
3. Reconnect before countdown ends.

### Expected Result

Player reconnects successfully and returns to Hero Selection.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-009

| Field    | Value                                |
| -------- | ------------------------------------ |
| Title    | Lock hero during the final countdown |
| Priority | High                                 |

### Test Steps

1. Wait until the countdown is nearly finished.
2. Lock the hero during the final seconds.

### Expected Result

Hero is locked successfully before the countdown expires.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-HERO-010

| Field    | Value                                          |
| -------- | ---------------------------------------------- |
| Title    | Select a hero already locked by another player |
| Priority | High                                           |

### Test Steps

1. Another player locks Hero A.
2. Attempt to select Hero A.

### Expected Result

Hero cannot be selected.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

# Execution Summary

| Result  | Count |
| ------- | ----: |
| PASS    |    10 |
| FAIL    |     0 |
| BLOCKED |     0 |

All Hero Selection test cases were executed successfully without any observed functional defects.
