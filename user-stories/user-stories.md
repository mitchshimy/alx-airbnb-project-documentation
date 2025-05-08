## 1. User Registration
**As a** new user,  
**I want to** register an account using email or OAuth,  
**so that** I can access the platform as a guest or host.  

**Acceptance Criteria**:  
- Email/password sign-up works.  
- Google/Facebook OAuth redirects correctly.  
- Role (guest/host) is assigned during registration.  

## 2. Property Listing Creation  
**As a** host,  
**I want to** add a new property listing with details (title, price, amenities, photos),  
**so that** guests can discover and book it.  

**Acceptance Criteria**:  
- Form validates required fields (title, price, location).  
- Images upload to cloud storage (AWS S3/Cloudinary).  
- Listing appears in search results after approval.  

## 3. Booking a Property  
**As a** guest,  
**I want to** book a property for specific dates and pay securely,  
**so that** I receive a confirmation and secure my stay.  

**Acceptance Criteria**:  
- Date conflicts are blocked.  
- Stripe/PayPal payment modal appears.  
- Confirmation email is sent post-booking.  

## 4. Cancellation & Refund  
**As a** guest,  
**I want to** cancel a booking and receive a refund based on the host's policy,  
**so that** I can recover costs for unexpected changes.  

**Acceptance Criteria**:  
- Cancellation triggers refund calculation (full/partial).  
- Host and guest receive cancellation notifications.  
- Payment status updates in the database.  

## 5. Admin Moderation  
**As an** admin,  
**I want to** approve new listings and resolve disputes,  
**so that** the platform remains safe and trustworthy.  

**Acceptance Criteria**:  
- Admin dashboard shows flagged listings/disputes.  
- Reject/approve actions update listing status.  
- Both parties receive dispute resolution notifications.  