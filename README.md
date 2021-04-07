# typed-react-form-yup

The yup validation wrapper to use with [typed-react-form](https://www.npmjs.com/package/typed-react-form).

## Usage

```tsx
import { yupValidator } from "typed-react-form-yup";

const FormSchema = yup.object({
    name: yup.string().required(),
    email: yup.string().required(),
});

const form = useForm({ name: "", email: "" }, yupValidator(FormSchema, { abortEarly: false }));

// ...
```
