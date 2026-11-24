# Customer Email and Chat Response Playbook

## Delayed delivery

**Email subject:** Update on your order {order_id}

**Email reply**

```
Dear {name},

I am sorry that your order {order_id} has not reached you on time - I understand how frustrating that is.

I have checked with our logistics partner and your parcel is now out for delivery. I will confirm the exact delivery slot with you by 6 PM today. If it does not arrive by tomorrow, we will ship a replacement or refund you in full, whichever you prefer.

Thank you for your patience.

Regards,
{agent}
{company} Customer Support
```

**Chat reply**

> Hi {name}, I am sorry about the delay on {order_id}. I have checked and it is out for delivery today. I will update you by 6 PM. If it is not delivered by tomorrow, I will arrange a replacement or refund. Thank you for waiting!

## Refund request

**Email subject:** Your refund request for order {order_id}

**Email reply**

```
Dear {name},

Thank you for contacting us, and I am sorry the product did not meet your expectations.

I have raised a refund for order {order_id} to your original payment method. It will reflect within 5-7 business days. I will send you the refund reference number today so you can track it.

Thank you for your understanding.

Regards,
{agent}
{company} Customer Support
```

**Chat reply**

> Hi {name}, I understand, and I am sorry the order did not work out. I have raised your refund for {order_id}. It will reflect in 5-7 business days and I will share the reference number today. Thanks for your patience!

## Billing error

**Email subject:** Correction on your bill for order {order_id}

**Email reply**

```
Dear {name},

I am sorry for the error on your bill - thank you for pointing it out. I understand how concerning an incorrect charge can be.

I have verified the transaction and confirmed that you were charged twice for {order_id}. I have raised a reversal for the extra amount and it will be credited within 3 business days. I will email you the corrected invoice by tomorrow.

Thank you for bringing this to us.

Regards,
{agent}
{company} Customer Support
```

**Chat reply**

> Hi {name}, I am sorry about the billing error. I have confirmed the duplicate charge on {order_id} and raised a reversal. It will be credited within 3 business days, and I will email the corrected invoice by tomorrow. Thank you for letting us know!

## Angry customer

**Email subject:** We are on it - your complaint about order {order_id}

**Email reply**

```
Dear {name},

I am truly sorry for the experience you have had. You have every right to be upset, and I understand how frustrating this has been.

I have taken ownership of your case myself. I have escalated it to our team lead for priority handling, and I will call or email you with a resolution within 24 hours. You will not need to repeat your issue again.

Thank you for giving us the chance to put this right.

Sincerely,
{agent}
{company} Customer Support
```

**Chat reply**

> Hi {name}, I am really sorry about this experience, and I understand your frustration. I have taken ownership of this and escalated it to my team lead for priority handling. I will come back to you within 24 hours with a resolution. Thank you for your patience.

## Wrong or damaged item

**Email subject:** Replacement for order {order_id}

**Email reply**

```
Dear {name},

I am sorry that you received the wrong or a damaged item. I understand how disappointing that is.

I have arranged a free pickup of the item and a replacement for {order_id}. The pickup will happen within 2 business days, and the replacement will ship once pickup is done. I will send you the tracking details today.

Thank you for your patience.

Regards,
{agent}
{company} Customer Support
```

**Chat reply**

> Hi {name}, I am sorry about that. I have arranged a free pickup and a replacement for {order_id}. Pickup will happen within 2 business days and I will share tracking details today. Thank you for letting us know!

## Escalation matrix

| Level   | Escalate to              | Trigger                                                                                            | Response expectation          |
|:--------|:-------------------------|:---------------------------------------------------------------------------------------------------|:------------------------------|
| L0      | Front-line agent         | Standard query within policy; refund up to Rs 2,000; first contact                                 | Resolve within SLA            |
| L1      | Team lead                | Customer asks for a supervisor; 2nd contact on same issue; SLA 75% elapsed; refund Rs 2,000-10,000 | Respond within 2 hours        |
| L2      | Billing / Finance team   | Duplicate or incorrect charge; payment gateway failure; refund above Rs 10,000                     | Respond within 1 business day |
| L2      | Logistics team           | Parcel lost or stuck more than 5 days; delivery partner dispute                                    | Respond within 1 business day |
| L3      | Customer Experience head | Repeated failure after L1/L2; public or social media complaint; goodwill gesture needed            | Respond within 4 hours        |
| L3      | Legal / Compliance       | Legal threat; data privacy or fraud concern; safety issue                                          | Immediate hand-off            |

