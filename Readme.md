# Project Phase 4

Authors: Radha Rungta, Ahana Talukdar, Apeksha Chandak, Bhavya Ram V

---

## Insert Functions

### 1. Insert Account
Adds a new account to the `Account` table. If bank details are included, they're inserted into the `Bank_Details` table. Collects info such as name, email, country, active devices, and bank account number.

### 2. Insert Subscription
Adds a subscription to an existing account. Inserts into `Subscription` and depending on the type (Mobile, Basic, Standard, Premium), into the respective table.

### 3. Insert Actor
Adds an actor to the `Actor` table with name, age, and country. `Actor_ID` is auto-generated.

### 4. Insert Show
Adds a new show via the `Content` and `Shows` tables, including title, description, country, rating, and number of seasons.

### 5. Insert Movie
Adds a movie to the `Movies` table after inserting general content info to the `Content` table.

---

## Retrieve Functions

### Selection Queries

#### 1. Subscription Status Report
Reports subscriptions that are either inactive or ending within 10 days. Categorizes them as Inactive or Ending Soon.

#### 2. Get Actors and Languages Worked In
Lists actors with languages they’ve performed in.

#### 3. Get All Movies of a Particular Genre
Retrieves all movies for a user-specified genre.

### Projection Queries

#### 4. Accounts with >3 Movies/Shows Watched
Displays account IDs of users who've watched more than 3 items.

#### 5. Get Content with Avg Rating > 8.5
Displays highly rated content, ordered by rating.

### Aggregate Queries

#### 6. Get Number of Actors per Content
Shows how many actors are linked to a specific content title.

#### 7. Get Account with Most Followers
Returns the account with the highest follower count.

#### 8. Get Total Hours Watched by Account
Sums total watch duration for a given user (by email).

### Search Queries

#### 9. Get Accounts Born Between 2000-2010
Filters accounts based on date of birth.

#### 10. Get Accounts with Name Containing 'REDDY'
Searches names for the substring 'REDDY'.

### Analysis Queries

#### 11. User Wrapped Summary
Summarizes user activity:
- Total watch time
- Most watched content
- Favorite genres
- Total reviews
- Most liked content
- Watch history over time

#### 12. Avg Rating by Country and Genre
Displays average ratings grouped by content origin and genre.

---

## Update Functions

### 1. Update Email
Updates a user’s email based on name and current email.

### 2. Update Account Type
Updates the `AccountType` (General/Kids) using the user’s name.

### 3. Update Bank Details
Updates bank info (account number, bank name, branch code) using email.

### 4. Update Mobile Subscription Price by Country
Updates subscription prices for specific countries and types.

---

## Delete Functions

### 1. Delete Account
Removes an account by email from the `Account` table.

### 2. Delete Subscription
Removes a subscription linked to an account email.

### 3. Delete Movie
Deletes a movie by title from the `Content` table.

### 4. Delete Show
Deletes a show by title from the `Content` table.

### 5. Delete Account Following
Removes a following relationship between two users based on emails.

---

Note: All functions include error handling and user-friendly messages for smooth execution.
