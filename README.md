[leacture numerical](https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/pages/week-1/)
[py](https://tbc-python.fossee.in/book-details/766/?utm_source=chatgpt.com)

# Numerical Methods

## 1. พื้นฐานและแนวคิดสำคัญ (Fundamentals & Concepts)

ก่อนเรียนเรื่องคำนวณ ต้องเข้าใจข้อจำกัดของคอมพิวเตอร์กับตัวเลขจริง

### หัวข้อหลัก
- ความคลาดเคลื่อนของตัวเลข (Types of Errors)
  - Round-off error – เกิดจากการปัดทศนิยมในคอมพิวเตอร์
  - Truncation error – เกิดจากการประมาณค่าด้วยสมการจำกัด
- ความแม่นยำ (Accuracy) และความเสถียร (Stability)
- การวิเคราะห์ข้อผิดพลาด (Error propagation)

---

## 2. การหาค่ารากของสมการ (Root Finding)

ใช้สำหรับแก้สมการที่ไม่มีคำตอบเชิงวิเคราะห์ เช่น f(x) = 0

### หัวข้อหลัก
- Bisection method
- False position (Regula Falsi)
- Newton-Raphson method
- Secant method
- Fixed-point iteration

ควรรู้: วิธีเลือกค่าเริ่มต้นและตรวจสอบการลู่เข้าสู่ค่ารากจริง

---

## 3. การแก้ระบบสมการเชิงเส้น (Solving Linear Systems)

ใช้เมื่อมีสมการหลายตัว เช่น ระบบ Ax = b

### หัวข้อหลัก
- Gaussian elimination
- Gauss-Jordan elimination
- LU decomposition
- Iterative methods
  - Jacobi method
  - Gauss-Seidel method
  - Successive Over-Relaxation (SOR)

ควรรู้: การวิเคราะห์ความเสถียรของระบบและค่า determinant

---

## 4. การประมาณค่าและการแทรกค่า (Interpolation & Approximation)

ใช้เมื่อมีข้อมูลบางจุด แล้วต้องการหาค่าระหว่างหรือสร้างสมการแทนข้อมูล

### หัวข้อหลัก
- Polynomial interpolation
  - Newton’s divided difference
  - Lagrange interpolation
- Spline interpolation
- Least squares regression (สมการเชิงเส้นที่เหมาะสมที่สุด)

ควรรู้: เปรียบเทียบระหว่างการใช้ polynomial ลำดับสูงกับ spline

---

## 5. การหาค่าอนุพันธ์และอินทิกรัลเชิงตัวเลข (Numerical Differentiation & Integration)

ใช้แทนการหาอนุพันธ์หรืออินทิกรัลที่ซับซ้อนเกินไปจะคำนวณตรง ๆ ไม่ได้

### Differentiation
- Forward difference
- Backward difference
- Central difference

### Integration
- Trapezoidal rule
- Simpson’s 1/3 rule
- Simpson’s 3/8 rule
- Romberg integration
- Gaussian quadrature

ควรรู้: วิธีเลือกจำนวนช่วง (step size) ให้เหมาะสมกับความแม่นยำ

---

## 6. การแก้สมการเชิงอนุพันธ์สามัญ (Ordinary Differential Equations – ODEs)

ใช้กับแบบจำลองที่มีการเปลี่ยนแปลงต่อเนื่อง เช่น การเคลื่อนที่หรือการเติบโตของประชากร

### หัวข้อหลัก
- Euler’s method
- Modified Euler method
- Runge-Kutta methods (2nd, 4th order)
- Predictor-Corrector methods
  - Adams-Bashforth
  - Adams-Moulton

ควรรู้: ความแตกต่างระหว่าง explicit และ implicit methods

---

## 7. การนำไปประยุกต์ใช้จริง (Implementation & Application)

ส่วนนี้คือสิ่งที่ทำให้ Numerical Method มีชีวิต

### การเขียนโปรแกรมแก้โจทย์ด้วยภาษา
- Python (เช่น NumPy, SciPy)
- MATLAB
- C/C++

### การวิเคราะห์ผลลัพธ์
- การสร้างกราฟ (Visualization)
- การวัดประสิทธิภาพของอัลกอริทึม (Time complexity, Stability)

---

## 8. เรื่องขั้นสูง (Advanced Topics)

เนื้อหาที่มักเรียนในชั้นปีสูงหรือระดับปริญญาโท

### หัวข้อหลัก
- การแก้สมการเชิงอนุพันธ์ย่อย (PDEs) เช่น Heat/Wave equation
- Numerical Optimization (เช่น Gradient Descent)
- Eigenvalues & Eigenvectors (เชิงตัวเลข)
- Finite Element Method (FEM)

---

## สรุปสิ่งที่ควรเข้าใจจริง

| หมวด | สิ่งที่ควรรู้ |
|-------|----------------|
| พื้นฐาน | Error, Stability |
| Root finding | Newton-Raphson, Bisection |
| Linear system | Gauss, LU, Iterative |
| Interpolation | Lagrange, Newton, Spline |
| Integration | Trapezoidal, Simpson |
| ODE | Euler, Runge-Kutta |
| Practical | เขียนโปรแกรมได้จริง |

---

Numerical Methods = คณิตศาสตร์ + การเขียนโปรแกรม + การแก้ปัญหาจริง
