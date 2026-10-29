MWANGAZA HARDWARE — PRODUCT BLUEPRINT

Version: 1.0.0
Status: Initial specification
Governing standard: PROJECT_CONSTITUTION.md
Visual standard: VISUAL_DESIGN_STANDARD.md
Operations standard: OPERATIONS_AND_MAINTENANCE.md

1. Product Vision

Build a professional, mobile-first website for Mwangaza Hardware that enables customers in Kenya to discover building and home products, select what they need, estimate costs where prices are confirmed, and request quotations.

The website will also support educational content, customer support and digital marketing.

The initial version will not process live payments.

2. Brand and Visual Direction

- Brand: Mwangaza Hardware.
- Visual identity: Modern African building brand.
- Primary color: Deep green.
- Accent color: Orange.
- Supporting colors: White, warm cream and charcoal.
- Logo: An approved geometric monogram incorporating the intended Mwangaza letterforms.
- Imagery: Relevant, realistic products and modern construction or home environments.
- Exclusion: No wood or natural-stone imagery in website graphics.
- Design priority: Mobile usability, clarity, performance and consistency.

Final logo assets, colors and typography must be approved before being treated as official brand assets.

3. Main Navigation

The website will provide access to:

1. Home.
2. Products.
3. Materials Calculator.
4. DIY Learning Centre.
5. Help and FAQs.
6. About Us.
7. Contact.

The basket or selected-items summary must be easy to find on mobile and desktop.

4. Product Categories

The main catalogue categories are:

1. Building Items.
2. Plumbing Appliances and Accessories.
3. Electrical Items.
4. Electronics Items.
5. Water Supply Items.
6. Interior Design Items.
7. Home Appliances.

Each category opens a dedicated view containing products assigned to that category.

Products must not appear in unrelated categories unless the business intentionally assigns them to more than one category.

5. Catalogue Requirements

Each product record should support:

- Unique product identifier.
- Product name.
- Main category and optional subcategory.
- Product image.
- Description.
- Brand, model or specifications where relevant.
- Selling unit.
- Confirmed price, if available.
- Availability status, if confirmed.
- Search keywords.
- Publication status.

A product may have a price marked as unavailable or quotation-required.

Demonstration products must be clearly labelled as sample data and must not be mistaken for actual store stock.

6. Product Browsing and Search

Customers must be able to:

- Open each category.
- Search by product name or relevant keyword.
- Filter by available category attributes where useful.
- Open a product detail view.
- Read the description and specifications.
- See the selling unit and confirmed price, if available.
- Add a product to their selection.
- Return to browsing without losing their selection.

Search and category browsing must remain available without AI services.

7. Product Selection and Quotation Basket

The first release will provide a selection basket, not live checkout.

Customers must be able to:

- Add products.
- Choose quantities.
- Change quantities.
- Remove products.
- Continue shopping.
- Review selected products.
- See applicable line totals and the estimated subtotal.
- Identify products requiring a quotation.
- Submit a quotation or enquiry request.

The basket should retain selections during ordinary navigation. Persistence across browser restarts may be added where appropriate, with privacy and device-sharing risks considered.

Calculation rules

Line amount = Quantity × Confirmed unit price.

Subtotal = Sum of eligible line amounts.

Do not present a final payable amount when prices, taxes, delivery charges or other required terms remain unconfirmed.

Clearly distinguish an estimate from a confirmed quotation, accepted order or payment.

8. Quotation and Enquiry Process

The customer should be able to provide the minimum necessary contact information and submit the selected products for a quotation.

The system must:

- Validate required fields.
- Display clear errors for invalid input.
- Confirm submission only after successful receipt.
- Prevent accidental duplicate submissions where practical.
- Protect enquiry records.
- Provide an alternative contact route if submission fails.
- Allow the store to verify prices, availability and terms before confirming the quotation.

The initial implementation may use a validated enquiry form or a controlled WhatsApp handoff. Successful delivery must be verified.

9. Materials Calculator

The calculator should use the same authoritative product and pricing information as the catalogue wherever applicable.

It must support suitable quantities, units, line amounts and totals.

The calculation rules must be documented and tested.

Tax, discounts and delivery charges may only be applied according to confirmed business rules. The calculator must not invent rates or silently treat unknown prices as zero.

10. DIY Learning Centre

The Learning Centre will provide useful, reviewed guidance for customers and fundis.

Possible topics include:

- Building-material selection.
- Plumbing products and fittings.
- Electrical-product basics and safety.
- Water storage and pumping.
- Interior finishes and lighting.
- Home-appliance selection.
- Material estimation and avoiding common purchasing mistakes.

Content must be accurate, readable on mobile and cautious about safety-critical work.

11. Support and Contact

The website will include:

- Help and FAQs.
- Verified store contact details.
- Approved WhatsApp contact.
- Approved Facebook and TikTok links.
- A basic website support experience.
- A fallback contact method when automation is unavailable.

AI and WhatsApp automation must be evaluated for privacy, provider eligibility, reliability and cost before activation.

12. Marketing Agency Functions

The project should support responsible marketing through:

- Search-engine optimization.
- Product and category landing pages.
- Educational content.
- Campaign tracking.
- Enquiry attribution.
- Website performance reporting.
- Sales attribution when supported by verified records.

Marketing costs, agency fees, store revenue and commissions must be accounted for separately.

13. Future Payments and Commission Management

Live payments are excluded from the initial release.

A later phase may introduce an approved payment provider, secure order management, payment reconciliation, commission calculation and commission reporting.

The business owner must approve the merchant account, settlement destination, commission agreement, provider fees and financial controls before activation.

Customer funds must not be routed through the agency's personal account.

14. Security and Privacy

- Do not expose secrets in public source code.
- Protect private enquiry and customer records.
- Validate inputs.
- Restrict access to administrative functions.
- Use HTTPS in production.
- Apply data minimization and appropriate privacy notices.
- Keep privileged operations server-side.
- Test the relevant security controls before launch.

15. Performance and Accessibility

- Mobile-first responsive design.
- Optimized images.
- Minimal unnecessary scripts and dependencies.
- Useful loading, empty, error and success states.
- Accessible labels, contrast and navigation.
- Testing on representative Android devices and browsers.
- Automated checks for relevant performance, accessibility and security requirements.

16. Acceptance Criteria

The initial website is not ready for release until:

- All seven categories are accessible.
- Category pages show the correct products.
- Product details display correctly.
- Search and category filters work.
- Customers can add, edit and remove selected items.
- Calculations use verified prices and correct units.
- Unpriced items can be included in quotation requests without fabricated totals.
- Enquiry submission and failure states are tested.
- The website works on mobile.
- Required automated tests pass.
- Applicable release gates in PROJECT_CONSTITUTION.md are satisfied.

17. Implementation Principle

Build in small, testable stages. Verify each feature before expanding the next. Preserve working functionality, document decisions, and do not declare a feature complete without evidence.
