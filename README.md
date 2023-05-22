# job-portal-android-system-app
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    private Button applyButton;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        applyButton = findViewById(R.id.applyButton);
        applyButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                applyForJob();
            }
        });
    }

    private void applyForJob() {
        // Perform the job application logic here

        // Display a toast message to indicate success
        Toast.makeText(this, "Job application submitted", Toast.LENGTH_SHORT).show();
    }
}
