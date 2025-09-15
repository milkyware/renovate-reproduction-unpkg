# UNPKG Support

Reproduction for **[Renovate discussion 36653](https://github.com/renovatebot/renovate/discussions/36653)**

## Current behavior

Renovate currently only supports the **[cdnjs](https://docs.renovatebot.com/modules/datasource/cdnjs/)** data source. UNPKG hosted libraries aren't updated.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Other Elements -->
    <link href="https://unpkg.com/bootstrap@5.3.7/dist/css/bootstrap.min.css" rel="stylesheet"> <!--Update package to next available version -->
</head>
<body>
    <!-- Other Elements -->
    <script src="https://unpkg.com/bootstrap@5.3.7/dist/js/bootstrap.bundle.min.js"></script> <!--Update package to next available version -->
</body>
</html>
```

## Expected behavior

Update the bootstrap package to **5.3.8** (at the time of writing)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Other Elements -->
    <link href="https://unpkg.com/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet"> <!--Updated to 5.3.8 -->
</head>
<body>
    <!-- Other Elements -->
    <script src="https://unpkg.com/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js"></script> <!--Updated to 5.3.8 -->
</body>
</html>
```

## Link to the Renovate issue or Discussion

Put your link to the Renovate issue or Discussion here.

## References

- [UNPKG](https://unpkg.com/)