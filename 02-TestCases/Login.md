# Login Test Suite

## Module Information

| Item             | Value              |
| ---------------- | ------------------ |
| Module           | Login              |
| Test Type        | Functional Testing |
| Tester           | Quang Minh         |
| Platform         | Android            |
| Total Test Cases | 5                  |
| Passed           | 5                  |
| Failed           | 0                  |
| Blocked          | 0                  |
| Test Result      | ✅ PASS            |

## Covered Requirements

| Requirement ID | Description                          |
| -------------- | ------------------------------------ |
| LOGIN-REQ-001  | User can log in with a valid account |
| LOGIN-REQ-002  | Invalid credentials are rejected     |
| LOGIN-REQ-003  | Network errors are handled correctly |

## Execution Summary

| Result  | Count |
| ------- | ----: |
| PASS    |     5 |
| FAIL    |     0 |
| BLOCKED |     0 |

All planned Login test cases were executed successfully without any observed defects.

**Module:** Login

**Testing Type:** Functional Testing

**Status:** Completed

Execution Date

2026-07-18

---

## AOV-TC-LOGIN-001

| Field         | Value                                                                             |
| ------------- | --------------------------------------------------------------------------------- |
| Title         | Login with a valid account                                                        |
| Priority      | High                                                                              |
| Preconditions | Game is installed. Internet connection is available. A valid game account exists. |
| Test Data     | Valid username and password                                                       |

### Test Steps

1. Launch Arena of Valor.
2. Enter a valid username.
3. Enter the correct password.
4. Tap **Login**.

### Expected Result

- Login is successful.
- The player is redirected to the main lobby.
- Player information is loaded correctly.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-LOGIN-002

| Field         | Value                             |
| ------------- | --------------------------------- |
| Title         | Login with an incorrect password  |
| Priority      | High                              |
| Preconditions | Internet connection is available. |
| Test Data     | Valid username + invalid password |

### Test Steps

1. Launch the game.
2. Enter a valid username.
3. Enter an incorrect password.
4. Tap **Login**.

### Expected Result

- Login fails.
- An appropriate error message is displayed.
- User remains on the login screen.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-LOGIN-003

| Field         | Value                                |
| ------------- | ------------------------------------ |
| Title         | Login without an Internet connection |
| Priority      | High                                 |
| Preconditions | Disable Wi-Fi and mobile data.       |

### Test Steps

1. Launch the game.
2. Enter a valid account.
3. Tap **Login**.

### Expected Result

- Login fails.
- A network error message is displayed.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-LOGIN-004

| Field         | Value                             |
| ------------- | --------------------------------- |
| Title         | Login with empty credentials      |
| Priority      | Medium                            |
| Preconditions | Internet connection is available. |

### Test Steps

1. Launch the game.
2. Leave username empty.
3. Leave password empty.
4. Tap **Login**.

### Expected Result

- Login is not processed.
- Validation message is displayed.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---

## AOV-TC-LOGIN-005

| Field         | Value                                    |
| ------------- | ---------------------------------------- |
| Title         | Login after reconnecting to the Internet |
| Priority      | Medium                                   |
| Preconditions | Start without Internet connection.       |

### Test Steps

1. Launch the game without Internet.
2. Turn on Wi-Fi.
3. Tap **Retry/Login**.

### Expected Result

- Connection is restored.
- Login succeeds.

### Actual Result

Matches the expected result.

**Status:** ✅ PASS

---
