CREATE TABLE public.operation  (
id BIGINT GENERATED ALWAYS AS IDENTITY PRIMARY KEY,
patient_id BIGINT,
doctor_id bigint,
FOREIGN KEY (patient_id) REFERENCES public.patient(id),
FOREIGN KEY (doctor_id) REFERENCES public.doctor(id)