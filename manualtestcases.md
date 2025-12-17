# Manual Test Cases for User Story US-ATC-02 — Add to Cart Functionality

### US-ATC-02-TC-001 — Add single item to cart (logged-in user)
- **Preconditions:** User is logged in and on the product detail page for an in-stock product. 
- **Test Data:**  
  - User: logged_in_user  
  - Product SKU: SKU-ADD-001  

#### Test Steps: 
1. Verify product name, price, and availability on the product detail page for SKU-ADD-001.  
2. Ensure the quantity is set to 1.  
3. Activate the Add to Cart control.  
4. Observe the cart indicator and open the cart page.

#### Expected Result:
- SKU-ADD-001 appears in the cart with quantity 1.  
- Cart count increments by 1.  
- Unit price matches product page.

**Ending Test Case**

---

### US-ATC-02-TC-002 — Add item to cart as guest (policy-dependent)
- **Preconditions:** User is not logged in and on the product detail page for an in-stock product.  
- **Test Data:**  
  - Product SKU: SKU-GUEST-001  

#### Test Steps:
1. On the product detail page for SKU-GUEST-001, activate the Add to Cart control.  
2. Observe whether the application allows a guest cart or prompts for sign-in.  
3. If allowed, open the cart page and verify contents; if prompted, note the prompt behavior.

#### Expected Result:
- If guest carts are supported, SKU-GUEST-001 is added and the cart count increments.  
- If login is required, the user is prompted to sign in and the item is not added until authenticated.

**Ending Test Case**