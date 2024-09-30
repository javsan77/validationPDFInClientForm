# validationPDFInClientForm
Simple Validation in field file of form (client side)
    <script>
        $('archivo').change(function(event) {
            const file = event.target.files[0]; 
            if (file && file.type !== 'application/pdf') { 
                alert('Por favor, suba un archivo PDF.');
                $(this).val('');
            }
        });
    </script>
