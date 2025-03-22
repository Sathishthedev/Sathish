import {  } from "@/components/ui/button"
import {  } from "@/components/ui/card"
import {
  
} from "@/components/ui/dropdown-menu"
import {   } from "@/components/ui/separator"
import {   } from "lucide-react"

export default function GitHubCard() {
  return (
    <Card className="w-full max-w-lg">
      <CardHeader className="grid grid-cols-[1fr_110px] items-start gap-4 space-y-0">
        <div className="space-y-1">
          <CardTitle>  </CardTitle>
          <CardDescription>
          < >
          </CardDescription>
        </div>
        <div className="flex items-center gap-1 rounded-md bg-secondary text-secondary-foreground">
          <Button variant="secondary" className="px-3 shadow-none">
            <Star className="w-4 h-4 mr-2" />
            Star
          </Button>
          <Separator orientation="vertical" className="h-[20px]" />
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button variant="secondary" className="px-2 shadow-none">
                <ChevronDown className="w-4 h-4 text-secondary-foreground" />
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent align="end" alignOffset={-5} className="w-[200px]" forceMount>
              <DropdownMenuLabel> </DropdownMenuLabel>
              <DropdownMenuSeparator />
              <DropdownMenuCheckboxItem checked> </DropdownMenuCheckboxItem>
              <DropdownMenuCheckboxItem> </DropdownMenuCheckboxItem>
              <DropdownMenuCheckboxItem> </DropdownMenuCheckboxItem>
              <DropdownMenuSeparator />
              <DropdownMenuItem>
                <Plus className="w-4 h-4 mr-2" /> Create List
              </DropdownMenuItem>
            </DropdownMenuContent>
          </DropdownMenu>
        </div>
      </CardHeader>
      <CardContent>
        <div className="flex flex-wrap gap-4 text-sm text-muted-foreground">
          <div className="flex items-center">
            <CircleDot className="w-3 h-3 mr-1 text-blue-500" />
            
          </div>
          <div className="flex items-center">
            <Star className="w-3 h-3 mr-1" />
            112k
          </div>
          <div className="flex items-center">
            <GitFork className="w-3 h-3 mr-1" />
            
          </div>
          <div> </div>
        </div>
      </CardContent>
    </Card>
  )
}

